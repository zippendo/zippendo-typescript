
# VerifyApiToken200Response


## Properties

Name | Type
------------ | -------------
`valid` | boolean
`tokenId` | string
`userId` | string
`orgId` | string
`scopes` | Array&lt;string&gt;
`expiresAt` | string

## Example

```typescript
import type { VerifyApiToken200Response } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "valid": true,
  "tokenId": tok_6e2fa83ij9,
  "userId": usr_9f3kd92ld0,
  "orgId": org_4d8af01qw2,
  "scopes": ["read:shipments"],
  "expiresAt": 2026-09-20T14:30:00.000Z,
} satisfies VerifyApiToken200Response

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as VerifyApiToken200Response
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


