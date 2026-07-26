
# CreateShippingQuoteRequestDestination


## Properties

Name | Type
------------ | -------------
`country` | string
`postalCode` | string
`province` | string
`city` | string
`address1` | string
`address2` | string

## Example

```typescript
import type { CreateShippingQuoteRequestDestination } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "country": DK,
  "postalCode": 1620,
  "province": ,
  "city": København,
  "address1": Vesterbrogade 1,
  "address2": 2. sal,
} satisfies CreateShippingQuoteRequestDestination

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShippingQuoteRequestDestination
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


