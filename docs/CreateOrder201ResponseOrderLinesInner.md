
# CreateOrder201ResponseOrderLinesInner


## Properties

Name | Type
------------ | -------------
`sku` | string
`name` | string
`quantity` | number
`unitPrice` | number
`totalPrice` | number
`currency` | string
`weight` | number
`weightUnit` | string
`variantId` | string
`productId` | string
`imageUrl` | string
`hsCode` | string
`countryOfOrigin` | string
`provinceOfOrigin` | string
`barcode` | string
`requiresShipping` | boolean
`taxable` | boolean
`giftCard` | boolean
`vendor` | string

## Example

```typescript
import type { CreateOrder201ResponseOrderLinesInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "sku": SKU-1042-BLK,
  "name": Wool Sweater,
  "quantity": 2,
  "unitPrice": 499,
  "totalPrice": 998,
  "currency": DKK,
  "weight": 0.5,
  "weightUnit": kg,
  "variantId": 44218900291,
  "productId": 8123456789,
  "imageUrl": https://cdn.example.dk/products/sweater.jpg,
  "hsCode": 611020,
  "countryOfOrigin": DK,
  "provinceOfOrigin": DK-84,
  "barcode": 5712345678901,
  "requiresShipping": true,
  "taxable": true,
  "giftCard": false,
  "vendor": Norse Knits,
} satisfies CreateOrder201ResponseOrderLinesInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateOrder201ResponseOrderLinesInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


