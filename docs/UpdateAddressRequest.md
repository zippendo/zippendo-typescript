
# UpdateAddressRequest


## Properties

Name | Type
------------ | -------------
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

## Example

```typescript
import type { UpdateAddressRequest } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Hovedlager,
  "attContact": Mette Hansen,
  "address1": Vesterbrogade 1,
  "address2": 2. sal,
  "zipcode": 1620,
  "city": København,
  "phone": +4533123456,
  "countryCode": DK,
  "state": Hovedstaden,
  "email": lager@example.dk,
  "customs": {"eori":"DK12345678"},
  "addressTypes": ["sender"],
} satisfies UpdateAddressRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UpdateAddressRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


