
# GetOrder200Response


## Properties

Name | Type
------------ | -------------
`id` | string
`orderNumber` | string
`externalId` | string
`customerName` | string
`customerEmail` | string
`shippingAddress` | [CreateOrder201ResponseShippingAddress](CreateOrder201ResponseShippingAddress.md)
`orderLines` | [Array&lt;CreateOrder201ResponseOrderLinesInner&gt;](CreateOrder201ResponseOrderLinesInner.md)
`subtotalAmount` | number
`totalAmount` | number
`currency` | string
`status` | string
`shippingRuleId` | string
`notes` | string
`externalData` | { [key: string]: any; }
`orderChannelId` | string
`orgId` | string
`createdAt` | string
`updatedAt` | string
`orderChannel` | [ListOrders200ResponseDataInnerOrderChannel](ListOrders200ResponseDataInnerOrderChannel.md)
`shippingRule` | [GetOrder200ResponseShippingRule](GetOrder200ResponseShippingRule.md)
`shipments` | [Array&lt;GetOrder200ResponseShipmentsInner&gt;](GetOrder200ResponseShipmentsInner.md)

## Example

```typescript
import type { GetOrder200Response } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": clz9k2f0a0003abcd9012mnop,
  "orderNumber": #1042,
  "externalId": 5012345678901,
  "customerName": Anna Jensen,
  "customerEmail": anna@example.dk,
  "shippingAddress": null,
  "orderLines": null,
  "subtotalAmount": 998,
  "totalAmount": 1047,
  "currency": DKK,
  "status": processing,
  "shippingRuleId": clz9k2f0a0002abcd5678ijkl,
  "notes": Leave at front desk,
  "externalData": null,
  "orderChannelId": clz9k2f0a0001abcd1234efgh,
  "orgId": clz9k2f0a0000abcd0000zzzz,
  "createdAt": 2026-06-22T14:30:00.000Z,
  "updatedAt": 2026-06-22T14:30:00.000Z,
  "orderChannel": null,
  "shippingRule": null,
  "shipments": null,
} satisfies GetOrder200Response

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GetOrder200Response
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


