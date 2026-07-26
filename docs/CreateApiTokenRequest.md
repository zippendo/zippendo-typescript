
# CreateApiTokenRequest


## Properties

Name | Type
------------ | -------------
`name` | string
`scopes` | Array&lt;string&gt;
`expiresInDays` | number

## Example

```typescript
import type { CreateApiTokenRequest } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Warehouse integration,
  "scopes": ["read:shipments","write:shipments"],
  "expiresInDays": 90,
} satisfies CreateApiTokenRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateApiTokenRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


