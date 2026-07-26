
# ListAvailableCarriers200ResponseInnerRequiredFieldsInner


## Properties

Name | Type
------------ | -------------
`name` | string
`key` | string
`type` | string
`options` | [Array&lt;ListCarrierProducts200ResponseInnerAdditionalParametersInnerOptionsInner&gt;](ListCarrierProducts200ResponseInnerAdditionalParametersInnerOptionsInner.md)
`description` | string
`required` | boolean

## Example

```typescript
import type { ListAvailableCarriers200ResponseInnerRequiredFieldsInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Customer number,
  "key": customerNumber,
  "type": string,
  "options": null,
  "description": Your PostNord customer number,
  "required": true,
} satisfies ListAvailableCarriers200ResponseInnerRequiredFieldsInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListAvailableCarriers200ResponseInnerRequiredFieldsInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


