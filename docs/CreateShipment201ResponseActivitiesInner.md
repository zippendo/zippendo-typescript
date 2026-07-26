
# CreateShipment201ResponseActivitiesInner


## Properties

Name | Type
------------ | -------------
`id` | string
`action` | string
`description` | string
`metadata` | any
`createdAt` | string

## Example

```typescript
import type { CreateShipment201ResponseActivitiesInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": act_1d2e3f4a,
  "action": created,
  "description": Shipment created,
  "metadata": null,
  "createdAt": 2026-06-22T14:30:00.000Z,
} satisfies CreateShipment201ResponseActivitiesInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShipment201ResponseActivitiesInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


