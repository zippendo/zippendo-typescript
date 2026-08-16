
# ListShippingRules200ResponseDataInnerCarrier


## Properties

Name | Type
------------ | -------------
`id` | string
`name` | string
`carrierSlug` | string
`config` | [{ [key: string]: ListCarriers200ResponseDataInnerConfigValue; }](ListCarriers200ResponseDataInnerConfigValue.md)
`orgId` | string
`brandId` | string
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { ListShippingRules200ResponseDataInnerCarrier } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": carr_01HZX9K2QF,
  "name": PostNord,
  "carrierSlug": postnord,
  "config": {"customerNumber":"123456"},
  "orgId": org_01HZX9K2QF,
  "brandId": brnd_8f3kd92ld0,
  "createdAt": 2026-06-22T09:00:00.000Z,
  "updatedAt": 2026-06-22T09:00:00.000Z,
} satisfies ListShippingRules200ResponseDataInnerCarrier

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListShippingRules200ResponseDataInnerCarrier
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


