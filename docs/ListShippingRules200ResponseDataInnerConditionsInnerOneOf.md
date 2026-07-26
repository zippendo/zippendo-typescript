
# ListShippingRules200ResponseDataInnerConditionsInnerOneOf


## Properties

Name | Type
------------ | -------------
`type` | string
`min` | number
`max` | number
`shippingPrice` | number
`currency` | string

## Example

```typescript
import type { ListShippingRules200ResponseDataInnerConditionsInnerOneOf } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "type": weight,
  "min": 0,
  "max": 5,
  "shippingPrice": 39,
  "currency": DKK,
} satisfies ListShippingRules200ResponseDataInnerConditionsInnerOneOf

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListShippingRules200ResponseDataInnerConditionsInnerOneOf
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


