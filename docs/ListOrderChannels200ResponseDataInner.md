
# ListOrderChannels200ResponseDataInner


## Properties

Name | Type
------------ | -------------
`id` | string
`name` | string
`type` | string
`enabled` | boolean
`role` | string
`brandId` | string
`hasCredentials` | boolean
`settings` | [ListOrderChannels200ResponseDataInnerSettings](ListOrderChannels200ResponseDataInnerSettings.md)
`webhooksEnabled` | boolean
`lastSyncAt` | Date
`lastSyncError` | string
`shippingRuleIds` | Array&lt;string&gt;
`orgId` | string
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { ListOrderChannels200ResponseDataInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": clz9k2f0a0001abcd1234efgh,
  "name": Anna's Shopify Store,
  "type": shopify,
  "enabled": true,
  "role": orders_and_rates,
  "brandId": brnd_8f3kd92ld0,
  "hasCredentials": true,
  "settings": null,
  "webhooksEnabled": true,
  "lastSyncAt": 2026-06-22T14:30Z,
  "lastSyncError": Invalid API credentials,
  "shippingRuleIds": ["clz9k2f0a0002abcd5678ijkl"],
  "orgId": clz9k2f0a0000abcd0000zzzz,
  "createdAt": 2026-06-22T14:30:00.000Z,
  "updatedAt": 2026-06-22T14:30:00.000Z,
} satisfies ListOrderChannels200ResponseDataInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListOrderChannels200ResponseDataInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


