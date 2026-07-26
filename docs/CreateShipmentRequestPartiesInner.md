
# CreateShipmentRequestPartiesInner


## Properties

Name | Type
------------ | -------------
`type` | string
`name` | string
`attention` | string
`address1` | string
`address2` | string
`postalCode` | string
`city` | string
`countryCode` | string
`email` | string
`phone` | string
`attributes` | [Array&lt;CreateShipmentRequestPartiesInnerAttributesInner&gt;](CreateShipmentRequestPartiesInnerAttributesInner.md)

## Example

```typescript
import type { CreateShipmentRequestPartiesInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "type": receiver,
  "name": Anna Jensen,
  "attention": Reception,
  "address1": Vesterbrogade 12,
  "address2": 2. sal,
  "postalCode": 1620,
  "city": København V,
  "countryCode": DK,
  "email": anna@example.dk,
  "phone": +4520123456,
  "attributes": null,
} satisfies CreateShipmentRequestPartiesInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShipmentRequestPartiesInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


