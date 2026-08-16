
# CreateOrgWebhook201Response


## Properties

Name | Type
------------ | -------------
`id` | string
`name` | string
`url` | string
`secret` | string
`events` | Array&lt;string&gt;
`isActive` | boolean
`brandId` | string
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { CreateOrgWebhook201Response } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": wh_clx1a2b3c4,
  "name": Order fulfilment notifier,
  "url": https://hooks.example.dk/zippendo,
  "secret": whsec_8f3a1c2b9d4e5f6a,
  "events": ["shipment.created"],
  "isActive": true,
  "brandId": brnd_8f3kd92ld0,
  "createdAt": 2026-06-01T09:30:00.000Z,
  "updatedAt": 2026-06-10T11:15:00.000Z,
} satisfies CreateOrgWebhook201Response

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateOrgWebhook201Response
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


