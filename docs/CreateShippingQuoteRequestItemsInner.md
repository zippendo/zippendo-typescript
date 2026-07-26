
# CreateShippingQuoteRequestItemsInner


## Properties

Name | Type
------------ | -------------
`name` | string
`sku` | string
`quantity` | number
`grams` | number
`price` | number
`productId` | string
`variantId` | string

## Example

```typescript
import type { CreateShippingQuoteRequestItemsInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Uld trøje,
  "sku": SKU-1001,
  "quantity": 2,
  "grams": 500,
  "price": 29900,
  "productId": prod_01HZX9K2QF,
  "variantId": var_01HZX9K2QF,
} satisfies CreateShippingQuoteRequestItemsInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShippingQuoteRequestItemsInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


