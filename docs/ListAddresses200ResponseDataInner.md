
# ListAddresses200ResponseDataInner


## Properties

Name | Type
------------ | -------------
`id` | string
`name` | string
`attContact` | string
`address1` | string
`address2` | string
`zipcode` | string
`city` | string
`phone` | string
`countryCode` | string
`state` | string
`email` | string
`customs` | { [key: string]: string; }
`addressTypes` | Array&lt;string&gt;
`orgId` | string
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { ListAddresses200ResponseDataInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": addr_01HZX9K2QF,
  "name": Hovedlager,
  "attContact": Mette Hansen,
  "address1": Vesterbrogade 1,
  "address2": 2. sal,
  "zipcode": 1620,
  "city": København,
  "phone": +4533123456,
  "countryCode": DK,
  "state": null,
  "email": lager@example.dk,
  "customs": {"eori":"DK12345678"},
  "addressTypes": ["sender"],
  "orgId": org_01HZX9K2QF,
  "createdAt": 2026-06-22T09:00:00.000Z,
  "updatedAt": 2026-06-22T09:00:00.000Z,
} satisfies ListAddresses200ResponseDataInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListAddresses200ResponseDataInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


