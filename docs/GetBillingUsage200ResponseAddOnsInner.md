
# GetBillingUsage200ResponseAddOnsInner


## Properties

Name | Type
------------ | -------------
`type` | string
`quantity` | number
`unitPrice` | number
`totalPrice` | number

## Example

```typescript
import type { GetBillingUsage200ResponseAddOnsInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "type": extra_carrier,
  "quantity": 2,
  "unitPrice": 9900,
  "totalPrice": 19800,
} satisfies GetBillingUsage200ResponseAddOnsInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GetBillingUsage200ResponseAddOnsInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


