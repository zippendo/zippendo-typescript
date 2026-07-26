
# ListCarrierProducts200ResponseInner


## Properties

Name | Type
------------ | -------------
`name` | string
`productId` | string
`type` | string
`description` | string
`availableCountries` | Array&lt;string&gt;
`availableSenderCountries` | Array&lt;string&gt;
`isServicePoint` | boolean
`isPickupAvailable` | boolean
`services` | [Array&lt;ListCarrierProducts200ResponseInnerServicesInner&gt;](ListCarrierProducts200ResponseInnerServicesInner.md)
`additionalParameters` | [Array&lt;ListCarrierProducts200ResponseInnerAdditionalParametersInner&gt;](ListCarrierProducts200ResponseInnerAdditionalParametersInner.md)
`weightLimits` | [ListCarrierProducts200ResponseInnerWeightLimits](ListCarrierProducts200ResponseInnerWeightLimits.md)

## Example

```typescript
import type { ListCarrierProducts200ResponseInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": PostNord MyPack Home,
  "productId": PNL13,
  "type": outbound,
  "description": Home delivery within Denmark,
  "availableCountries": null,
  "availableSenderCountries": null,
  "isServicePoint": false,
  "isPickupAvailable": true,
  "services": null,
  "additionalParameters": null,
  "weightLimits": null,
} satisfies ListCarrierProducts200ResponseInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListCarrierProducts200ResponseInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


