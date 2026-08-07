# Zippendo TypeScript SDK

Official TypeScript/JavaScript client for the [Zippendo](https://zippendo.com) shipping & logistics
API. Built on the Fetch API, so it runs in Node 18+, Deno, Bun, browsers, and edge runtimes. Every
request and response is fully typed.

## Install

```sh
npm install @zippendo/sdk
```

## Authentication

Create an API token in your Zippendo dashboard (**Settings → API tokens**). It is a Bearer token
prefixed with `zipp_`. Pass it as `accessToken`:

```ts
import { Configuration } from "@zippendo/sdk"

const config = new Configuration({ accessToken: process.env.ZIPPENDO_API_TOKEN })
```

The base URL defaults to `https://api.zippendo.com` — you don't need to set it.

## Resources & clients

The API is split into resource clients — `ShipmentsApi`, `OrdersApi`, `CarriersApi`, `AddressesApi`,
`RulesApi`, `WebhooksApi`, `TokensApi`, and more. Construct the ones you need with your `config`:

```ts
import { Configuration, ShipmentsApi, OrdersApi } from "@zippendo/sdk"

const config = new Configuration({ accessToken: process.env.ZIPPENDO_API_TOKEN })
const shipments = new ShipmentsApi(config)
const orders = new OrdersApi(config)
```

## The `orgId` parameter

Every call takes an `orgId` (your organization ID, found in the dashboard). It is explicit on each
call by design: one API token can be granted access to multiple organizations, and `orgId` selects
which one the request acts on.

## Brands

A brand is a sub-account inside an organization: one company running several consumer-facing labels
(say Pitaya and Kiwi) keeps each label's orders and shipments separate, with its own company name,
address and logo on the documents its shipments produce. Scope a request to one brand with the
`X-Zippendo-Brand` header, whose value is the brand's ID or slug.

The header is not a method parameter — it applies uniformly to every operation, so set it once on the
`Configuration` and every call made with it inherits it:

```ts
const pitaya = new Configuration({
  accessToken: process.env.ZIPPENDO_API_TOKEN,
  headers: { "X-Zippendo-Brand": "pitaya" }, // brand ID or slug
})

const shipments = new ShipmentsApi(pitaya)
await shipments.listShipments({ orgId: "org_8f3kd92ld0", limit: 50 }) // Pitaya's shipments only
```

To address two brands from one process, build a `Configuration` per brand and pass each to its own
resource clients. Omit the header and the request covers the whole organization — the behaviour of
every existing token. A header naming a brand that does not exist in the organization is rejected
with `404 BRAND_NOT_FOUND`.

An API token created with a `brandId` is permanently confined to that brand and needs no header.
Sending `X-Zippendo-Brand` naming a *different* brand on such a token is refused with
`403 BRAND_ACCESS_DENIED` — the binding is never widened.

Creating, updating and deleting brands is done in the Zippendo dashboard; brand management is not
part of this SDK.

## Listing & pagination

List endpoints accept `page` (1-based) and `limit`, and return a page with `data` plus
`total`, `page`, `limit`, and `totalPages`:

```ts
const result = await shipments.listShipments({ orgId: "org_8f3kd92ld0", page: 1, limit: 50 })
console.log(result.data)                       // Shipment[]
console.log(result.total, result.totalPages)   // pagination metadata
```

## Creating resources

```ts
const order = await orders.createOrder({
  orgId: "org_8f3kd92ld0",
  createOrderRequest: {
    orderNumber: "1001",
    orderChannelId: "chan_7d2k1",
    orderLines: [{ name: "T-shirt", quantity: 2 }],
  },
})
console.log(order.id)
```

See [`./docs`](./docs) for the full request/response shape of every operation.

## Error handling

Non-2xx responses throw a `ResponseError`. The body is Zippendo's canonical
`{ code, error, message }` — branch on the machine-readable `code`:

```ts
import { ResponseError } from "@zippendo/sdk"

try {
  await shipments.getShipment({ orgId: "org_8f3kd92ld0", shipmentId: "shp_missing" })
} catch (err) {
  if (err instanceof ResponseError) {
    const body = await err.response.json()
    console.error(body.code, body.message) // e.g. "SHIPMENT_NOT_FOUND"
  } else {
    throw err
  }
}
```

## Configuration

Point the client at a different environment by overriding `basePath`:

```ts
const config = new Configuration({
  accessToken: process.env.ZIPPENDO_API_TOKEN,
  basePath: "https://staging.api.zippendo.com",
})
```

## Reference

Full per-endpoint and per-model documentation is in [`./docs`](./docs). Hosted reference:
<https://www.zippendo.com/docs/api-reference/overview>.

## License

[MIT](./LICENSE.md)
