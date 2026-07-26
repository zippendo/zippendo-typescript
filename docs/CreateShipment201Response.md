
# CreateShipment201Response


## Properties

Name | Type
------------ | -------------
`id` | string
`reference` | string
`addressId` | string
`servicePointId` | string
`parties` | [Array&lt;CreateShipment201ResponsePartiesInner&gt;](CreateShipment201ResponsePartiesInner.md)
`type` | string
`carrierSettings` | [ListShipments200ResponseDataInnerCarrierSettings](ListShipments200ResponseDataInnerCarrierSettings.md)
`parcels` | [Array&lt;CreateShipment201ResponseParcelsInner&gt;](CreateShipment201ResponseParcelsInner.md)
`pickupDetails` | [CreateShipment201ResponsePickupDetails](CreateShipment201ResponsePickupDetails.md)
`termOfTrade` | string
`documents` | [Array&lt;CreateShipment201ResponseDocumentsInner&gt;](CreateShipment201ResponseDocumentsInner.md)
`errors` | [Array&lt;CreateShipment201ResponseErrorsInner&gt;](CreateShipment201ResponseErrorsInner.md)
`tracking` | [CreateShipment201ResponseTracking](CreateShipment201ResponseTracking.md)
`status` | string
`orgId` | string
`orderId` | string
`shippingRuleId` | string
`shippingRule` | [CreateShipment201ResponseShippingRule](CreateShipment201ResponseShippingRule.md)
`labelPrinterId` | string
`documentPrinterId` | string
`logs` | [Array&lt;CreateShipment201ResponseLogsInner&gt;](CreateShipment201ResponseLogsInner.md)
`activities` | [Array&lt;CreateShipment201ResponseActivitiesInner&gt;](CreateShipment201ResponseActivitiesInner.md)
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { CreateShipment201Response } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": shp_4d9e7a2f,
  "reference": ORDER-1042,
  "addressId": addr_7e8f9a0b,
  "servicePointId": sp_pn_4521,
  "parties": null,
  "type": outbound,
  "carrierSettings": null,
  "parcels": null,
  "pickupDetails": null,
  "termOfTrade": DAP,
  "documents": null,
  "errors": null,
  "tracking": null,
  "status": pending,
  "orgId": org_1a2b3c4d,
  "orderId": ord_5e6f7a8b,
  "shippingRuleId": rule_3c4d5e6f,
  "shippingRule": null,
  "labelPrinterId": prn_label_01,
  "documentPrinterId": prn_doc_01,
  "logs": null,
  "activities": null,
  "createdAt": 2026-06-22T14:30:00.000Z,
  "updatedAt": 2026-06-22T14:30:00.000Z,
} satisfies CreateShipment201Response

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShipment201Response
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


