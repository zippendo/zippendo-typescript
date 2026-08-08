
# ListOrgBrands200ResponseDataInner


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
`id` | string
`orgId` | string
`name` | string
`slug` | string
`useOrgCustoms` | boolean
`logoUrl` | string
`archivedAt` | string
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { ListOrgBrands200ResponseDataInner } from '@zippendo/sdk'

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
  "id": brnd_8f3kd92ld0,
  "orgId": org_8f3kd92ld0,
  "name": Acme,
  "slug": acme,
  "useOrgCustoms": true,
  "logoUrl": /orgs/org_1/brands/brnd_1/logo,
  "archivedAt": 2026-08-05T10:00:00.000Z,
  "createdAt": 2026-06-22T14:30:00.000Z,
  "updatedAt": 2026-06-22T14:30:00.000Z,
} satisfies ListOrgBrands200ResponseDataInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListOrgBrands200ResponseDataInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


