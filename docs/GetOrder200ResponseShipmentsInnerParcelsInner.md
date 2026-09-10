
# GetOrder200ResponseShipmentsInnerParcelsInner


## Properties

Name | Type
------------ | -------------
`id` | string
`weight` | number
`weightUnit` | string
`dimensions` | [CreateShipment201ResponseParcelsInnerDimensions](CreateShipment201ResponseParcelsInnerDimensions.md)
`orderLines` | [Array&lt;GetOrder200ResponseShipmentsInnerParcelsInnerOrderLinesInner&gt;](GetOrder200ResponseShipmentsInnerParcelsInnerOrderLinesInner.md)

## Example

```typescript
import type { GetOrder200ResponseShipmentsInnerParcelsInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": prc_5a6b7c8d,
  "weight": 2.5,
  "weightUnit": kg,
  "dimensions": null,
  "orderLines": null,
} satisfies GetOrder200ResponseShipmentsInnerParcelsInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GetOrder200ResponseShipmentsInnerParcelsInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


