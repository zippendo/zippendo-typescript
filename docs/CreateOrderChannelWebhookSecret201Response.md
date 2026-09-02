
# CreateOrderChannelWebhookSecret201Response


## Properties

Name | Type
------------ | -------------
`secret` | string
`webhookUrl` | string
`createdAt` | Date

## Example

```typescript
import type { CreateOrderChannelWebhookSecret201Response } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "secret": zwhs_XeVJ1n8vJZbJ0N3mYQ2fV0dK9cA5tR7uW4pL6sH8gB0,
  "webhookUrl": https://api.zippendo.com/webhooks/order-channels/clz9k2f0a0001abcd1234efgh,
  "createdAt": 2026-09-02T14:30Z,
} satisfies CreateOrderChannelWebhookSecret201Response

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateOrderChannelWebhookSecret201Response
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


