
# CreateShippingRuleRequestConditionsInnerOneOf2


## Properties

Name | Type
------------ | -------------
`type` | string
`priceType` | string
`min` | number
`max` | number
`shippingPrice` | number
`currency` | string

## Example

```typescript
import type { CreateShippingRuleRequestConditionsInnerOneOf2 } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "type": priceRange,
  "priceType": total,
  "min": 0,
  "max": 499,
  "shippingPrice": 49,
  "currency": DKK,
} satisfies CreateShippingRuleRequestConditionsInnerOneOf2

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShippingRuleRequestConditionsInnerOneOf2
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


