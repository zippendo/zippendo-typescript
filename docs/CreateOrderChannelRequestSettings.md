
# CreateOrderChannelRequestSettings


## Properties

Name | Type
------------ | -------------
`useWebhooks` | boolean
`siteUrl` | string
`autoFulfill` | boolean
`autoSync` | boolean
`syncIntervalMinutes` | number
`autoShipOnCreate` | boolean
`defaultCarrierId` | string
`defaultProductId` | string
`defaultAddressId` | string
`shippingMethodMappings` | [Array&lt;CreateOrderChannelRequestSettingsShippingMethodMappingsInner&gt;](CreateOrderChannelRequestSettingsShippingMethodMappingsInner.md)
`syncOnlyUnfulfilled` | boolean
`syncOrdersSince` | Date
`servicePointCount` | number

## Example

```typescript
import type { CreateOrderChannelRequestSettings } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "useWebhooks": true,
  "siteUrl": https://butik.dk,
  "autoFulfill": true,
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
} satisfies CreateOrderChannelRequestSettings

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateOrderChannelRequestSettings
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


