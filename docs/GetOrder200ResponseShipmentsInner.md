
# GetOrder200ResponseShipmentsInner


## Properties

Name | Type
------------ | -------------
`id` | string
`reference` | string
`status` | string
`type` | string
`tracking` | [CreateShipment201ResponseTracking](CreateShipment201ResponseTracking.md)
`carrierSettings` | [ListShipments200ResponseDataInnerCarrierSettings](ListShipments200ResponseDataInnerCarrierSettings.md)
`createdAt` | string
`updatedAt` | string
`shippingRuleId` | string
`documents` | [Array&lt;CreateShipment201ResponseDocumentsInner&gt;](CreateShipment201ResponseDocumentsInner.md)

## Example

```typescript
import type { GetOrder200ResponseShipmentsInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": shp_4d9e7a2f,
  "reference": ORDER-1042,
  "status": pending,
  "type": outbound,
  "tracking": null,
  "carrierSettings": null,
  "createdAt": 2026-06-22T14:30:00.000Z,
  "updatedAt": 2026-06-22T14:30:00.000Z,
  "shippingRuleId": clz9k2f0a0002abcd5678ijkl,
  "documents": null,
} satisfies GetOrder200ResponseShipmentsInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GetOrder200ResponseShipmentsInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


