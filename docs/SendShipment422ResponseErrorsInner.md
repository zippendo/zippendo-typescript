
# SendShipment422ResponseErrorsInner


## Properties

Name | Type
------------ | -------------
`code` | string
`message` | string

## Example

```typescript
import type { SendShipment422ResponseErrorsInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "code": INVALID_POSTAL_CODE,
  "message": Receiver postal code is invalid for the selected product.,
} satisfies SendShipment422ResponseErrorsInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SendShipment422ResponseErrorsInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


