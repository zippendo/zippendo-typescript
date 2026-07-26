
# ListShipments200Response


## Properties

Name | Type
------------ | -------------
`data` | [Array&lt;ListShipments200ResponseDataInner&gt;](ListShipments200ResponseDataInner.md)
`total` | number
`page` | number
`limit` | number
`totalPages` | number

## Example

```typescript
import type { ListShipments200Response } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "data": null,
  "total": 137,
  "page": 1,
  "limit": 20,
  "totalPages": 7,
} satisfies ListShipments200Response

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListShipments200Response
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


