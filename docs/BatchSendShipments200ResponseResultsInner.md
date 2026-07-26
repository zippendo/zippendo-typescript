
# BatchSendShipments200ResponseResultsInner


## Properties

Name | Type
------------ | -------------
`shipmentId` | string
`status` | string
`code` | string
`message` | string
`errors` | [Array&lt;SendShipment422ResponseErrorsInner&gt;](SendShipment422ResponseErrorsInner.md)

## Example

```typescript
import type { BatchSendShipments200ResponseResultsInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "shipmentId": shp_01H8XABC123,
  "status": sent,
  "code": CARRIER_ERROR,
  "message": Shipment must be in pending or error status to be sent,
  "errors": null,
} satisfies BatchSendShipments200ResponseResultsInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BatchSendShipments200ResponseResultsInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


