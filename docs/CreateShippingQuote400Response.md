
# CreateShippingQuote400Response


## Properties

Name | Type
------------ | -------------
`error` | string
`message` | string

## Example

```typescript
import type { CreateShippingQuote400Response } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "error": Bad Request,
  "message": Invalid destination country,
} satisfies CreateShippingQuote400Response

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShippingQuote400Response
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


