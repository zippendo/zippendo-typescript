
# TrackShipment200ResponseEventsInner


## Properties

Name | Type
------------ | -------------
`id` | string
`status` | string
`carrierStatus` | string
`description` | string
`location` | string
`occurredAt` | string

## Example

```typescript
import type { TrackShipment200ResponseEventsInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": trk_7a8b9c0d,
  "status": in_transit,
  "carrierStatus": INFORMED,
  "description": The shipment is on its way.,
  "location": København,
  "occurredAt": 2026-06-22T14:30:00.000Z,
} satisfies TrackShipment200ResponseEventsInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TrackShipment200ResponseEventsInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


