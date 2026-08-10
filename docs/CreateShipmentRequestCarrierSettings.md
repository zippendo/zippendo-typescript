
# CreateShipmentRequestCarrierSettings


## Properties

Name | Type
------------ | -------------
`carrierId` | string
`productId` | string
`services` | Array&lt;string&gt;
`additionalParameters` | [{ [key: string]: CreateShippingRuleRequestAdditionalParametersValue; }](CreateShippingRuleRequestAdditionalParametersValue.md)

## Example

```typescript
import type { CreateShipmentRequestCarrierSettings } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "carrierId": car_pn_001,
  "productId": prod_mypack_home,
  "services": ["A7"],
  "additionalParameters": {"notificationEmail":"anna@example.dk"},
} satisfies CreateShipmentRequestCarrierSettings

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShipmentRequestCarrierSettings
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


