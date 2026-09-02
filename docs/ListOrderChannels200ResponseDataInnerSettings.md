
# ListOrderChannels200ResponseDataInnerSettings

Channel settings (webhook secret and checkout token hash omitted).

## Properties

Name | Type
------------ | -------------
`useWebhooks` | boolean
`webhookId` | string
`webhookIds` | Array&lt;number&gt;
`webhookSecretCreatedAt` | Date
`siteUrl` | string
`autoFulfill` | boolean
`checkoutTokenCreatedAt` | Date
`autoSync` | boolean
`syncIntervalMinutes` | number
`autoShipOnCreate` | boolean
`defaultCarrierId` | string
`defaultProductId` | string
`defaultAddressId` | string
`shippingMethodMappings` | [Array&lt;ListOrderChannels200ResponseDataInnerSettingsShippingMethodMappingsInner&gt;](ListOrderChannels200ResponseDataInnerSettingsShippingMethodMappingsInner.md)
`syncOnlyUnfulfilled` | boolean
`syncOrdersSince` | Date
`servicePointCount` | number

## Example

```typescript
import type { ListOrderChannels200ResponseDataInnerSettings } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "useWebhooks": true,
  "webhookId": gid://shopify/WebhookSubscription/12345,
  "webhookIds": [12,13,14],
  "webhookSecretCreatedAt": 2026-06-22T14:30Z,
  "siteUrl": https://butik.dk,
  "autoFulfill": true,
  "checkoutTokenCreatedAt": 2026-06-22T14:30Z,
  "autoSync": false,
  "syncIntervalMinutes": 15,
  "autoShipOnCreate": false,
  "defaultCarrierId": clz9k2f0a0006abcd1357yzab,
  "defaultProductId": postnord-home-delivery,
  "defaultAddressId": clz9k2f0a0005abcd7890uvwx,
  "shippingMethodMappings": [{"match":"GLS Hjemmelevering","shippingRuleId":"clz9k2f0a0007abcd2468qrst"}],
  "syncOnlyUnfulfilled": true,
  "syncOrdersSince": 2026-05-22T00:00Z,
  "servicePointCount": 6,
} satisfies ListOrderChannels200ResponseDataInnerSettings

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListOrderChannels200ResponseDataInnerSettings
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


