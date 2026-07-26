
# CreateShippingRuleRequestConditionsInnerOneOf4


## Properties

Name | Type
------------ | -------------
`type` | string
`shippingPrice` | number
`currency` | string

## Example

```typescript
import type { CreateShippingRuleRequestConditionsInnerOneOf4 } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "type": flatRate,
  "shippingPrice": 39,
  "currency": DKK,
} satisfies CreateShippingRuleRequestConditionsInnerOneOf4

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShippingRuleRequestConditionsInnerOneOf4
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


