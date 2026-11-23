
# ListCarrierProducts200ResponseInnerDangerousGoodsInner


## Properties

Name | Type
------------ | -------------
`kind` | string
`serviceId` | string
`parameters` | [ListCarrierProducts200ResponseInnerDangerousGoodsInnerParameters](ListCarrierProducts200ResponseInnerDangerousGoodsInnerParameters.md)
`ownedParameters` | Array&lt;string&gt;
`singleParcel` | boolean

## Example

```typescript
import type { ListCarrierProducts200ResponseInnerDangerousGoodsInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "kind": limited_quantity,
  "serviceId": LQ,
  "parameters": null,
  "ownedParameters": ["lqUnNumber","lqPackagingGroup","lqClass","lqCode","lqSubWeight"],
  "singleParcel": true,
} satisfies ListCarrierProducts200ResponseInnerDangerousGoodsInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListCarrierProducts200ResponseInnerDangerousGoodsInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


