
# CreateOrgWebhookRequest


## Properties

Name | Type
------------ | -------------
`name` | string
`url` | string
`events` | Array&lt;string&gt;
`isActive` | boolean
`brandId` | string

## Example

```typescript
import type { CreateOrgWebhookRequest } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Order fulfilment notifier,
  "url": https://hooks.example.dk/zippendo,
  "events": ["shipment.created","tracking.updated"],
  "isActive": true,
  "brandId": brnd_8f3kd92ld0,
} satisfies CreateOrgWebhookRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateOrgWebhookRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


