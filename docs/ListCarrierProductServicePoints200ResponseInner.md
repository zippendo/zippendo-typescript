
# ListCarrierProductServicePoints200ResponseInner


## Properties

Name | Type
------------ | -------------
`lat` | number
`lng` | number
`name` | string
`servicePointId` | string
`openingHours` | Array&lt;string&gt;
`description` | string
`distance` | number
`address` | [ListCarrierProductServicePoints200ResponseInnerAddress](ListCarrierProductServicePoints200ResponseInnerAddress.md)

## Example

```typescript
import type { ListCarrierProductServicePoints200ResponseInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "lat": 55.6761,
  "lng": 12.5683,
  "name": PostNord Pakkeshop Netto,
  "servicePointId": 1234567,
  "openingHours": null,
  "description": Located inside Netto supermarket,
  "distance": 320,
  "address": null,
} satisfies ListCarrierProductServicePoints200ResponseInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListCarrierProductServicePoints200ResponseInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


