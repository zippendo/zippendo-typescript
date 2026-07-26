
# BatchSendShipments200ResponseSummary

Aggregate counts for the batch.

## Properties

Name | Type
------------ | -------------
`total` | number
`sent` | number
`failed` | number

## Example

```typescript
import type { BatchSendShipments200ResponseSummary } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "total": 3,
  "sent": 2,
  "failed": 1,
} satisfies BatchSendShipments200ResponseSummary

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BatchSendShipments200ResponseSummary
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


