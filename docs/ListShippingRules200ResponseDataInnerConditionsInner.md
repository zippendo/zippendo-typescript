
# ListShippingRules200ResponseDataInnerConditionsInner


## Properties

Name | Type
------------ | -------------
`type` | string
`min` | number
`max` | number
`shippingPrice` | number
`currency` | string
`priceType` | string
`operator` | string
`value` | number

## Example

```typescript
import type { ListShippingRules200ResponseDataInnerConditionsInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "type": weight,
  "min": 0,
  "max": 499,
  "shippingPrice": 39,
  "currency": DKK,
  "priceType": total,
  "operator": gte,
  "value": 3,
} satisfies ListShippingRules200ResponseDataInnerConditionsInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListShippingRules200ResponseDataInnerConditionsInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


