
# SendShipment422Response


## Properties

Name | Type
------------ | -------------
`code` | string
`error` | string
`message` | string
`errors` | [Array&lt;SendShipment422ResponseErrorsInner&gt;](SendShipment422ResponseErrorsInner.md)

## Example

```typescript
import type { SendShipment422Response } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "code": CARRIER_GLS_WRONG_ADDRESS,
  "error": Carrier Error,
  "message": Shipment could not be booked with PostNord.,
  "errors": null,
} satisfies SendShipment422Response

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SendShipment422Response
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


