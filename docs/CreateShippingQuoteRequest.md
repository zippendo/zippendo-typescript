
# CreateShippingQuoteRequest


## Properties

Name | Type
------------ | -------------
`destination` | [CreateShippingQuoteRequestDestination](CreateShippingQuoteRequestDestination.md)
`items` | [Array&lt;CreateShippingQuoteRequestItemsInner&gt;](CreateShippingQuoteRequestItemsInner.md)
`currency` | string
`totalPriceCents` | number

## Example

```typescript
import type { CreateShippingQuoteRequest } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "destination": null,
  "items": [{"name":"Uld trøje","quantity":2,"grams":500,"price":29900}],
  "currency": DKK,
  "totalPriceCents": 59800,
} satisfies CreateShippingQuoteRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShippingQuoteRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


