
# CreateShippingRuleRequestAdditionalParametersValueAnyOf


## Properties

Name | Type
------------ | -------------
`id` | string
`name` | string
`address` | string
`coordinates` | [Array&lt;ListShippingRules200ResponseDataInnerAdditionalParametersValueAnyOfCoordinatesInner&gt;](ListShippingRules200ResponseDataInnerAdditionalParametersValueAnyOfCoordinatesInner.md)

## Example

```typescript
import type { CreateShippingRuleRequestAdditionalParametersValueAnyOf } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": sp_pn_4521,
  "name": Føtex Nørrebro,
  "address": Nørrebrogade 20, 2200 København N,
  "coordinates": [55.6987,12.5501],
} satisfies CreateShippingRuleRequestAdditionalParametersValueAnyOf

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShippingRuleRequestAdditionalParametersValueAnyOf
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


