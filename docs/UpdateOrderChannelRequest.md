
# UpdateOrderChannelRequest


## Properties

Name | Type
------------ | -------------
`brandId` | string
`name` | string
`enabled` | boolean
`role` | string
`credentials` | { [key: string]: any; }
`settings` | [UpdateOrderChannelRequestSettings](UpdateOrderChannelRequestSettings.md)
`shippingRuleIds` | Array&lt;string&gt;

## Example

```typescript
import type { UpdateOrderChannelRequest } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "brandId": brnd_8f3kd92ld0,
  "name": Anna's Shopify Store,
  "enabled": true,
  "role": orders_and_rates,
  "credentials": null,
  "settings": null,
  "shippingRuleIds": ["clz9k2f0a0002abcd5678ijkl"],
} satisfies UpdateOrderChannelRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UpdateOrderChannelRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


