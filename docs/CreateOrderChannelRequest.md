
# CreateOrderChannelRequest


## Properties

Name | Type
------------ | -------------
`name` | string
`type` | string
`brandId` | string
`enabled` | boolean
`settings` | [CreateOrderChannelRequestSettings](CreateOrderChannelRequestSettings.md)

## Example

```typescript
import type { CreateOrderChannelRequest } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Anna's webshop,
  "type": custom,
  "brandId": brnd_8f3kd92ld0,
  "enabled": true,
  "settings": null,
} satisfies CreateOrderChannelRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateOrderChannelRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


