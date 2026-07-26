
# ListCarrierProducts200ResponseInnerWeightLimits

Allowed weight range for parcels using this product

## Properties

Name | Type
------------ | -------------
`min` | number
`max` | number
`unit` | string

## Example

```typescript
import type { ListCarrierProducts200ResponseInnerWeightLimits } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "min": 0.1,
  "max": 35,
  "unit": kg,
} satisfies ListCarrierProducts200ResponseInnerWeightLimits

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListCarrierProducts200ResponseInnerWeightLimits
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


