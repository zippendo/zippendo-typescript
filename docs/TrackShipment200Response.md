
# TrackShipment200Response


## Properties

Name | Type
------------ | -------------
`trackingNumber` | string
`trackingUrl` | string
`currentStatus` | string
`estimatedDelivery` | string
`events` | [Array&lt;TrackShipment200ResponseEventsInner&gt;](TrackShipment200ResponseEventsInner.md)

## Example

```typescript
import type { TrackShipment200Response } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "trackingNumber": 00370724710000012345,
  "trackingUrl": https://tracking.postnord.com/00370724710000012345,
  "currentStatus": delivered,
  "estimatedDelivery": 2026-06-23T12:00:00.000Z,
  "events": null,
} satisfies TrackShipment200Response

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TrackShipment200Response
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


