
# CreateShipment201ResponseLogsInner


## Properties

Name | Type
------------ | -------------
`id` | string
`direction` | string
`request` | any
`response` | any
`statusCode` | number
`error` | string
`duration` | number
`createdAt` | string

## Example

```typescript
import type { CreateShipment201ResponseLogsInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": log_6f7a8b9c,
  "direction": outbound,
  "request": null,
  "response": null,
  "statusCode": 200,
  "error": Connection timed out,
  "duration": 342,
  "createdAt": 2026-06-22T14:30:00.000Z,
} satisfies CreateShipment201ResponseLogsInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShipment201ResponseLogsInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


