
# GetOrderChannelWebhookStatus200Response


## Properties

Name | Type
------------ | -------------
`enabled` | boolean
`webhookUrl` | string
`webhooks` | [Array&lt;GetOrderChannelWebhookStatus200ResponseWebhooksInner&gt;](GetOrderChannelWebhookStatus200ResponseWebhooksInner.md)

## Example

```typescript
import type { GetOrderChannelWebhookStatus200Response } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "enabled": true,
  "webhookUrl": https://api.zippendo.dk/webhooks/order-channels/clz9k2f0a0001abcd1234efgh,
  "webhooks": null,
} satisfies GetOrderChannelWebhookStatus200Response

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GetOrderChannelWebhookStatus200Response
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


