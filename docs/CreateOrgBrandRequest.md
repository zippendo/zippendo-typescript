
# CreateOrgBrandRequest


## Properties

Name | Type
------------ | -------------
`companyName` | string
`vatNumber` | string
`customs` | { [key: string]: string; }
`addressLine1` | string
`addressLine2` | string
`city` | string
`postalCode` | string
`country` | string
`primaryColor` | string
`secondaryColor` | string
`name` | string
`slug` | string
`useOrgCustoms` | boolean

## Example

```typescript
import type { CreateOrgBrandRequest } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "companyName": Acme ApS,
  "vatNumber": DK12345678,
  "customs": {"eori":"DK12345678"},
  "addressLine1": Vestergade 12,
  "addressLine2": 3. sal,
  "city": København,
  "postalCode": 1456,
  "country": DK,
  "primaryColor": #1D4ED8,
  "secondaryColor": #F59E0B,
  "name": Acme,
  "slug": acme,
  "useOrgCustoms": true,
} satisfies CreateOrgBrandRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateOrgBrandRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


