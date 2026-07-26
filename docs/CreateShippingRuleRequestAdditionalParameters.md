
# CreateShippingRuleRequestAdditionalParameters

Carrier-specific extra parameters. Accepts EITHER the `{ key: value }` object (preferred) OR the legacy `[{ name, val }]` array, so you can migrate on your own schedule. Each key / `name` is the carrier parameter `key` from the product\'s `additionalParameters[].key` (e.g. `returnFunctionality`).

## Properties

Name | Type
------------ | -------------

## Example

```typescript
import type { CreateShippingRuleRequestAdditionalParameters } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
} satisfies CreateShippingRuleRequestAdditionalParameters

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShippingRuleRequestAdditionalParameters
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


