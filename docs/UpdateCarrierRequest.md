
# UpdateCarrierRequest


## Properties

Name | Type
------------ | -------------
`name` | string
`carrierSlug` | string
`config` | [{ [key: string]: ListCarriers200ResponseDataInnerConfigValue; }](ListCarriers200ResponseDataInnerConfigValue.md)

## Example

```typescript
import type { UpdateCarrierRequest } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": GLS,
  "carrierSlug": gls,
  "config": {"customerNumber":"123456"},
} satisfies UpdateCarrierRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UpdateCarrierRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


