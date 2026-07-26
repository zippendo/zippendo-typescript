
# ListOrgWebhooks200ResponseDataInner


## Properties

Name | Type
------------ | -------------
`id` | string
`name` | string
`url` | string
`events` | Array&lt;string&gt;
`isActive` | boolean
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { ListOrgWebhooks200ResponseDataInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": wh_clx1a2b3c4,
  "name": Order fulfilment notifier,
  "url": https://hooks.example.dk/zippendo,
  "events": ["shipment.created"],
  "isActive": true,
  "createdAt": 2026-06-01T09:30:00.000Z,
  "updatedAt": 2026-06-10T11:15:00.000Z,
} satisfies ListOrgWebhooks200ResponseDataInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListOrgWebhooks200ResponseDataInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


