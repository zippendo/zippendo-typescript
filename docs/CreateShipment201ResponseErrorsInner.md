
# CreateShipment201ResponseErrorsInner


## Properties

Name | Type
------------ | -------------
`id` | string
`carrier` | string
`code` | string
`message` | string
`createdAt` | string

## Example

```typescript
import type { CreateShipment201ResponseErrorsInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": err_2b3c4d5e,
  "carrier": PostNord,
  "code": INVALID_POSTAL_CODE,
  "message": Receiver postal code is invalid for the selected product.,
  "createdAt": 2026-06-22T14:30:00.000Z,
} satisfies CreateShipment201ResponseErrorsInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShipment201ResponseErrorsInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


