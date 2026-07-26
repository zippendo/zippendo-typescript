
# ListCarrierProductServicePointsRequest


## Properties

Name | Type
------------ | -------------
`address1` | string
`address2` | string
`postalCode` | string
`state` | string
`city` | string
`countryCode` | string

## Example

```typescript
import type { ListCarrierProductServicePointsRequest } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "address1": Vesterbrogade 1,
  "address2": 2. sal,
  "postalCode": 1620,
  "state": null,
  "city": København,
  "countryCode": DK,
} satisfies ListCarrierProductServicePointsRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListCarrierProductServicePointsRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


