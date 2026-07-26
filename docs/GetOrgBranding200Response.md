
# GetOrgBranding200Response


## Properties

Name | Type
------------ | -------------
`primaryColor` | string
`secondaryColor` | string
`logoUrl` | string

## Example

```typescript
import type { GetOrgBranding200Response } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "primaryColor": #1D4ED8,
  "secondaryColor": #F59E0B,
  "logoUrl": /orgs/org_123/branding/logo,
} satisfies GetOrgBranding200Response

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GetOrgBranding200Response
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


