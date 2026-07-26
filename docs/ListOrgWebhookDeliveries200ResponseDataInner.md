
# ListOrgWebhookDeliveries200ResponseDataInner


## Properties

Name | Type
------------ | -------------
`id` | string
`webhookId` | string
`event` | string
`payload` | any
`statusCode` | number
`response` | string
`duration` | number
`success` | boolean
`attempt` | number
`error` | string
`createdAt` | string

## Example

```typescript
import type { ListOrgWebhookDeliveries200ResponseDataInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": whd_clx9z8y7x6,
  "webhookId": wh_clx1a2b3c4,
  "event": shipment.created,
  "payload": {"id":"shp_123"},
  "statusCode": 200,
  "response": OK,
  "duration": 142,
  "success": true,
  "attempt": 1,
  "error": null,
  "createdAt": 2026-06-10T11:16:00.000Z,
} satisfies ListOrgWebhookDeliveries200ResponseDataInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListOrgWebhookDeliveries200ResponseDataInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


