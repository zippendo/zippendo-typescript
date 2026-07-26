
# CreateOrderRequest


## Properties

Name | Type
------------ | -------------
`orderNumber` | string
`externalId` | string
`orderChannelId` | string
`customerName` | string
`customerEmail` | string
`shippingAddress` | [CreateOrderRequestShippingAddress](CreateOrderRequestShippingAddress.md)
`orderLines` | [Array&lt;CreateOrderRequestOrderLinesInner&gt;](CreateOrderRequestOrderLinesInner.md)
`subtotalAmount` | number
`totalAmount` | number
`currency` | string
`notes` | string
`externalData` | { [key: string]: any; }

## Example

```typescript
import type { CreateOrderRequest } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "orderNumber": #1042,
  "externalId": 5012345678901,
  "orderChannelId": clz9k2f0a0001abcd1234efgh,
  "customerName": Anna Jensen,
  "customerEmail": anna@example.dk,
  "shippingAddress": null,
  "orderLines": null,
  "subtotalAmount": 998,
  "totalAmount": 1047,
  "currency": DKK,
  "notes": Leave at front desk,
  "externalData": null,
} satisfies CreateOrderRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateOrderRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


