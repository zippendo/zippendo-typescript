
# ListCarriers200ResponseDataInner


## Properties

Name | Type
------------ | -------------
`id` | string
`name` | string
`carrierSlug` | string
`config` | [{ [key: string]: ListCarriers200ResponseDataInnerConfigValue; }](ListCarriers200ResponseDataInnerConfigValue.md)
`orgId` | string
`brandId` | string
`createdAt` | string
`updatedAt` | string
`logo` | string
`brandColor` | string
`deprecated` | boolean
`deprecationMessage` | string

## Example

```typescript
import type { ListCarriers200ResponseDataInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": carr_01HZX9K2QF,
  "name": PostNord,
  "carrierSlug": postnord,
  "config": {"customerNumber":"123456"},
  "orgId": org_01HZX9K2QF,
  "brandId": brnd_8f3kd92ld0,
  "createdAt": 2026-06-22T09:00:00.000Z,
  "updatedAt": 2026-06-22T09:00:00.000Z,
  "logo": https://cdn.zippendo.com/logos/postnord.svg,
  "brandColor": #005BAA,
  "deprecated": true,
  "deprecationMessage": The standalone Instabox API is deprecated. Migrate to the Instabee-powered Instabox integration.,
} satisfies ListCarriers200ResponseDataInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListCarriers200ResponseDataInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


