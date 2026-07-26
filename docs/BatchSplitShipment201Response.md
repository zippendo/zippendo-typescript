
# BatchSplitShipment201Response


## Properties

Name | Type
------------ | -------------
`originalShipment` | [CreateShipment201Response](CreateShipment201Response.md)
`newShipments` | [Array&lt;CreateShipment201Response&gt;](CreateShipment201Response.md)

## Example

```typescript
import type { BatchSplitShipment201Response } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "originalShipment": null,
  "newShipments": null,
} satisfies BatchSplitShipment201Response

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BatchSplitShipment201Response
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


