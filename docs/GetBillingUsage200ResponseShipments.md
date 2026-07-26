
# GetBillingUsage200ResponseShipments


## Properties

Name | Type
------------ | -------------
`used` | number
`included` | number
`overage` | number
`overageCharges` | number

## Example

```typescript
import type { GetBillingUsage200ResponseShipments } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "used": 1240,
  "included": 1000,
  "overage": 240,
  "overageCharges": 36000,
} satisfies GetBillingUsage200ResponseShipments

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GetBillingUsage200ResponseShipments
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


