
# CreateShipment201ResponseParcelsInnerOrderLinesInner


## Properties

Name | Type
------------ | -------------
`id` | string
`sku` | string
`quantity` | number
`description` | string
`unitPrice` | number
`currency` | string
`vatPercent` | number
`location` | string
`countryOfOrigin` | string
`tarrifNumber` | string

## Example

```typescript
import type { CreateShipment201ResponseParcelsInnerOrderLinesInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": ol_9c1d2e3f,
  "sku": SKU-1024,
  "quantity": 2,
  "description": Wool sweater, navy,
  "unitPrice": 299.95,
  "currency": DKK,
  "vatPercent": 25,
  "location": A-12-3,
  "countryOfOrigin": DK,
  "tarrifNumber": 61101100,
} satisfies CreateShipment201ResponseParcelsInnerOrderLinesInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShipment201ResponseParcelsInnerOrderLinesInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


