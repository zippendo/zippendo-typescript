
# CreateShipment201ResponseDocumentsInner


## Properties

Name | Type
------------ | -------------
`id` | string
`shipmentId` | string
`documentType` | string
`format` | string
`content` | string
`size` | string
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { CreateShipment201ResponseDocumentsInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": doc_8f3a2b1c,
  "shipmentId": shp_4d9e7a2f,
  "documentType": label,
  "format": pdf,
  "content": JVBERi0xLjQKJeLjz9MKMS...,
  "size": 100X150,
  "createdAt": 2026-06-22T14:30:00.000Z,
  "updatedAt": 2026-06-22T14:30:00.000Z,
} satisfies CreateShipment201ResponseDocumentsInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShipment201ResponseDocumentsInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


