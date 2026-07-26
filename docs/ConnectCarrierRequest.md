
# ConnectCarrierRequest


## Properties

Name | Type
------------ | -------------
`name` | string
`carrierSlug` | string
`config` | [{ [key: string]: ListCarriers200ResponseDataInnerConfigValue; }](ListCarriers200ResponseDataInnerConfigValue.md)

## Example

```typescript
import type { ConnectCarrierRequest } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": PostNord,
  "carrierSlug": postnord,
  "config": {"customerNumber":"123456"},
} satisfies ConnectCarrierRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ConnectCarrierRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


