
# ListOrders200ResponseDataInner


## Properties

Name | Type
------------ | -------------
`id` | string
`orderNumber` | string
`customerName` | string
`customerEmail` | string
`status` | string
`subtotalAmount` | number
`totalAmount` | number
`currency` | string
`shipmentCount` | number
`orderChannel` | [ListOrders200ResponseDataInnerOrderChannel](ListOrders200ResponseDataInnerOrderChannel.md)
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { ListOrders200ResponseDataInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": clz9k2f0a0003abcd9012mnop,
  "orderNumber": #1042,
  "customerName": Anna Jensen,
  "customerEmail": anna@example.dk,
  "status": processing,
  "subtotalAmount": 998,
  "totalAmount": 1047,
  "currency": DKK,
  "shipmentCount": 1,
  "orderChannel": null,
  "createdAt": 2026-06-22T14:30:00.000Z,
  "updatedAt": 2026-06-22T14:30:00.000Z,
} satisfies ListOrders200ResponseDataInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListOrders200ResponseDataInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


