
# CreateShipment201ResponsePickupDetails


## Properties

Name | Type
------------ | -------------
`date` | string
`from` | string
`to` | string
`instruction` | string

## Example

```typescript
import type { CreateShipment201ResponsePickupDetails } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "date": 2026-06-22,
  "from": 08:00:00,
  "to": 16:00:00,
  "instruction": Ring the bell at the loading dock.,
} satisfies CreateShipment201ResponsePickupDetails

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShipment201ResponsePickupDetails
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


