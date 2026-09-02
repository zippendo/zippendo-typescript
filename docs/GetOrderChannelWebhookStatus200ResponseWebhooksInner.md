
# GetOrderChannelWebhookStatus200ResponseWebhooksInner


## Properties

Name | Type
------------ | -------------
`id` | number
`topic` | string
`address` | string
`createdAt` | string
`deliveryUrl` | string
`status` | string

## Example

```typescript
import type { GetOrderChannelWebhookStatus200ResponseWebhooksInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1234567890,
  "topic": ORDERS_CREATE,
  "address": https://api.zippendo.dk/webhooks/order-channels/clz9k2f0a0001abcd1234efgh,
  "createdAt": 2026-06-22T14:30:00.000Z,
  "deliveryUrl": https://api.zippendo.dk/webhooks/order-channels/clz9k2f0a0001abcd1234efgh,
  "status": active,
} satisfies GetOrderChannelWebhookStatus200ResponseWebhooksInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GetOrderChannelWebhookStatus200ResponseWebhooksInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


