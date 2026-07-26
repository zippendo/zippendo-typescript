
# ListCarrierProducts200ResponseInnerAdditionalParametersInner


## Properties

Name | Type
------------ | -------------
`name` | string
`key` | string
`type` | string
`options` | [Array&lt;ListCarrierProducts200ResponseInnerAdditionalParametersInnerOptionsInner&gt;](ListCarrierProducts200ResponseInnerAdditionalParametersInnerOptionsInner.md)
`description` | string
`isRequired` | boolean
`requiredService` | Array&lt;string&gt;

## Example

```typescript
import type { ListCarrierProducts200ResponseInnerAdditionalParametersInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Return Mode,
  "key": returnFunctionality,
  "type": enum,
  "options": null,
  "description": Instruction shown to the delivery driver,
  "isRequired": false,
  "requiredService": null,
} satisfies ListCarrierProducts200ResponseInnerAdditionalParametersInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListCarrierProducts200ResponseInnerAdditionalParametersInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


