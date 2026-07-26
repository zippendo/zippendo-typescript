
# ListApiTokens200ResponseDataInner


## Properties

Name | Type
------------ | -------------
`id` | string
`name` | string
`tokenPrefix` | string
`scopes` | Array&lt;string&gt;
`lastUsedAt` | string
`expiresAt` | string
`createdAt` | string
`createdBy` | [ListApiTokens200ResponseDataInnerCreatedBy](ListApiTokens200ResponseDataInnerCreatedBy.md)

## Example

```typescript
import type { ListApiTokens200ResponseDataInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": tok_6e2fa83ij9,
  "name": Warehouse integration,
  "tokenPrefix": zipp_live_8f,
  "scopes": ["read:shipments","write:shipments"],
  "lastUsedAt": 2026-06-22T14:30:00.000Z,
  "expiresAt": 2026-09-20T14:30:00.000Z,
  "createdAt": 2026-06-22T14:30:00.000Z,
  "createdBy": null,
} satisfies ListApiTokens200ResponseDataInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListApiTokens200ResponseDataInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


