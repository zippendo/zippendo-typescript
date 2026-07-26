
# UpdateOrgRequest


## Properties

Name | Type
------------ | -------------
`name` | string
`slug` | string
`description` | string
`currency` | string
`vatNumber` | string
`overageEnabled` | boolean
`billingEmail` | string
`companyName` | string
`addressLine1` | string
`addressLine2` | string
`city` | string
`postalCode` | string
`country` | string
`customs` | { [key: string]: string; }

## Example

```typescript
import type { UpdateOrgRequest } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Nordic Logistics ApS,
  "slug": nordic-logistics,
  "description": Parcel and freight logistics across the Nordics,
  "currency": DKK,
  "vatNumber": DK12345678,
  "overageEnabled": false,
  "billingEmail": billing@nordic-logistics.dk,
  "companyName": Nordic Logistics ApS,
  "addressLine1": Havnegade 12,
  "addressLine2": 3. sal,
  "city": København,
  "postalCode": 1058,
  "country": DK,
  "customs": null,
} satisfies UpdateOrgRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UpdateOrgRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


