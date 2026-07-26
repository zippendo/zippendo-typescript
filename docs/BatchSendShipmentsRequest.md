
# BatchSendShipmentsRequest


## Properties

Name | Type
------------ | -------------
`shipmentIds` | Array&lt;string&gt;

## Example

```typescript
import type { BatchSendShipmentsRequest } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "shipmentIds": ["shp_01H8XABC123","shp_01H8XDEF456"],
} satisfies BatchSendShipmentsRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BatchSendShipmentsRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


