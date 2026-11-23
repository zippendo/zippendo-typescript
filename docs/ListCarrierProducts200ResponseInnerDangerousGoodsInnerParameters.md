
# ListCarrierProducts200ResponseInnerDangerousGoodsInnerParameters

Which additional parameters carry the details of the goods. Absent ones are not sent.

## Properties

Name | Type
------------ | -------------
`unNumber` | string
`hazardClass` | string
`packingGroup` | string
`properShippingName` | string
`weightGramsPerParcel` | string
`weightKg` | string
`weightKgPerParcel` | string

## Example

```typescript
import type { ListCarrierProducts200ResponseInnerDangerousGoodsInnerParameters } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "unNumber": lqUnNumber,
  "hazardClass": lqClass,
  "packingGroup": lqPackagingGroup,
  "properShippingName": adrDescription,
  "weightGramsPerParcel": lqSubWeight,
  "weightKg": adrWeight,
  "weightKgPerParcel": dangerousGoodsLqWeight,
} satisfies ListCarrierProducts200ResponseInnerDangerousGoodsInnerParameters

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListCarrierProducts200ResponseInnerDangerousGoodsInnerParameters
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


