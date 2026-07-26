
# CreateShipmentRequest


## Properties

Name | Type
------------ | -------------
`reference` | string
`addressId` | string
`servicePointId` | string
`parties` | [Array&lt;CreateShipmentRequestPartiesInner&gt;](CreateShipmentRequestPartiesInner.md)
`type` | string
`carrierSettings` | [CreateShipmentRequestCarrierSettings](CreateShipmentRequestCarrierSettings.md)
`parcels` | [Array&lt;CreateShipmentRequestParcelsInner&gt;](CreateShipmentRequestParcelsInner.md)
`pickupDetails` | [CreateShipmentRequestPickupDetails](CreateShipmentRequestPickupDetails.md)
`termOfTrade` | string
`status` | string
`orderId` | string
`labelPrinterId` | string
`documentPrinterId` | string

## Example

```typescript
import type { CreateShipmentRequest } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "reference": ORDER-1042,
  "addressId": addr_7e8f9a0b,
  "servicePointId": sp_pn_4521,
  "parties": null,
  "type": outbound,
  "carrierSettings": null,
  "parcels": null,
  "pickupDetails": null,
  "termOfTrade": DAP,
  "status": pending,
  "orderId": ord_5e6f7a8b,
  "labelPrinterId": prn_label_01,
  "documentPrinterId": prn_doc_01,
} satisfies CreateShipmentRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShipmentRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


