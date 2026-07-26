
# GetOrg200Response


## Properties

Name | Type
------------ | -------------
`id` | string
`name` | string
`slug` | string
`description` | string
`currency` | string
`vatNumber` | string
`billingEmail` | string
`companyName` | string
`addressLine1` | string
`addressLine2` | string
`city` | string
`postalCode` | string
`country` | string
`customs` | { [key: string]: string; }
`createdAt` | string
`updatedAt` | string
`count` | [GetOrg200ResponseCount](GetOrg200ResponseCount.md)

## Example

```typescript
import type { GetOrg200Response } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": org_4d8af01qw2,
  "name": Nordic Logistics ApS,
  "slug": nordic-logistics,
  "description": Parcel and freight logistics across the Nordics,
  "currency": DKK,
  "vatNumber": DK12345678,
  "billingEmail": billing@nordic-logistics.dk,
  "companyName": Nordic Logistics ApS,
  "addressLine1": Havnegade 12,
  "addressLine2": 3. sal,
  "city": København,
  "postalCode": 1058,
  "country": DK,
  "customs": {"eori":"DK12345678"},
  "createdAt": 2026-06-22T14:30:00.000Z,
  "updatedAt": 2026-06-22T14:30:00.000Z,
  "count": null,
} satisfies GetOrg200Response

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GetOrg200Response
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


