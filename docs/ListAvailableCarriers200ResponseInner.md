
# ListAvailableCarriers200ResponseInner


## Properties

Name | Type
------------ | -------------
`name` | string
`slug` | string
`group` | string
`description` | string
`logo` | string
`brandColor` | string
`learnMoreUrl` | string
`requiredFields` | [Array&lt;ListAvailableCarriers200ResponseInnerRequiredFieldsInner&gt;](ListAvailableCarriers200ResponseInnerRequiredFieldsInner.md)
`optionalFields` | [Array&lt;ListAvailableCarriers200ResponseInnerRequiredFieldsInner&gt;](ListAvailableCarriers200ResponseInnerRequiredFieldsInner.md)
`deprecated` | boolean
`deprecationMessage` | string

## Example

```typescript
import type { ListAvailableCarriers200ResponseInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": PostNord,
  "slug": postnord,
  "group": Nordic,
  "description": Nordic postal and parcel carrier,
  "logo": https://cdn.zippendo.com/carriers/postnord.svg,
  "brandColor": #0072CE,
  "learnMoreUrl": https://www.postnord.dk,
  "requiredFields": null,
  "optionalFields": null,
  "deprecated": true,
  "deprecationMessage": The standalone Instabox API is deprecated. Migrate to the Instabee-powered Instabox integration.,
} satisfies ListAvailableCarriers200ResponseInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListAvailableCarriers200ResponseInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


