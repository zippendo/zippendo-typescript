
# SplitShipmentRequest


## Properties

Name | Type
------------ | -------------
`parcelId` | string
`orderLineIds` | Array&lt;string&gt;
`carrierId` | string
`productId` | string
`services` | Array&lt;string&gt;
`additionalParameters` | { [key: string]: any; }
`reference` | string

## Example

```typescript
import type { SplitShipmentRequest } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "parcelId": prc_5a6b7c8d,
  "orderLineIds": ["ol_9c1d2e3f"],
  "carrierId": car_pn_001,
  "productId": prod_mypack_home,
  "services": ["A7"],
  "additionalParameters": {"notificationEmail":"anna@example.dk"},
  "reference": ORDER-1042-split,
} satisfies SplitShipmentRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SplitShipmentRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


