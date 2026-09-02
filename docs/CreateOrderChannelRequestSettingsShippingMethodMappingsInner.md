
# CreateOrderChannelRequestSettingsShippingMethodMappingsInner


## Properties

Name | Type
------------ | -------------
`match` | string
`shippingRuleId` | string
`servicePointSelection` | string

## Example

```typescript
import type { CreateOrderChannelRequestSettingsShippingMethodMappingsInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "match": GLS Hjemmelevering,
  "shippingRuleId": clz9k2f0a0007abcd2468qrst,
  "servicePointSelection": nearest,
} satisfies CreateOrderChannelRequestSettingsShippingMethodMappingsInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateOrderChannelRequestSettingsShippingMethodMappingsInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


