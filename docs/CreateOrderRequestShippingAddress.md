
# CreateOrderRequestShippingAddress

Destination shipping address.

## Properties

Name | Type
------------ | -------------
`name` | string
`attention` | string
`company` | string
`address1` | string
`address2` | string
`city` | string
`province` | string
`provinceCode` | string
`postalCode` | string
`country` | string
`countryCode` | string
`phone` | string
`email` | string

## Example

```typescript
import type { CreateOrderRequestShippingAddress } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Anna Jensen,
  "attention": c/o Reception,
  "company": Jensen Design ApS,
  "address1": Nørregade 12,
  "address2": 2. sal,
  "city": København,
  "province": Hovedstaden,
  "provinceCode": DK-84,
  "postalCode": 1165,
  "country": Denmark,
  "countryCode": DK,
  "phone": +45 12 34 56 78,
  "email": anna@example.dk,
} satisfies CreateOrderRequestShippingAddress

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateOrderRequestShippingAddress
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


