
# ListShipments200ResponseDataInner


## Properties

Name | Type
------------ | -------------
`id` | string
`reference` | string
`type` | string
`carrierSettings` | [ListShipments200ResponseDataInnerCarrierSettings](ListShipments200ResponseDataInnerCarrierSettings.md)
`status` | string
`brandId` | string
`address` | [ListShipments200ResponseDataInnerAddress](ListShipments200ResponseDataInnerAddress.md)
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { ListShipments200ResponseDataInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": shp_4d9e7a2f,
  "reference": ORDER-1042,
  "type": outbound,
  "carrierSettings": null,
  "status": pending,
  "brandId": brnd_8f3kd92ld0,
  "address": null,
  "createdAt": 2026-06-22T14:30:00.000Z,
  "updatedAt": 2026-06-22T14:30:00.000Z,
} satisfies ListShipments200ResponseDataInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListShipments200ResponseDataInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


