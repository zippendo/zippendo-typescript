
# UpdateOrderRequest


## Properties

Name | Type
------------ | -------------
`orderNumber` | string
`customerName` | string
`customerEmail` | string
`shippingAddress` | [CreateOrderRequestShippingAddress](CreateOrderRequestShippingAddress.md)
`orderLines` | [Array&lt;CreateOrderRequestOrderLinesInner&gt;](CreateOrderRequestOrderLinesInner.md)
`subtotalAmount` | number
`totalAmount` | number
`currency` | string
`notes` | string
`status` | string
`shippingRuleId` | string

## Example

```typescript
import type { UpdateOrderRequest } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "orderNumber": #1042,
  "customerName": Anna Jensen,
  "customerEmail": anna@example.dk,
  "shippingAddress": null,
  "orderLines": null,
  "subtotalAmount": 998,
  "totalAmount": 1047,
  "currency": DKK,
  "notes": Leave at front desk,
  "status": processing,
  "shippingRuleId": clz9k2f0a0002abcd5678ijkl,
} satisfies UpdateOrderRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UpdateOrderRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


