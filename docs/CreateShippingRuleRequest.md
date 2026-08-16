
# CreateShippingRuleRequest


## Properties

Name | Type
------------ | -------------
`name` | string
`description` | string
`direction` | string
`carrierId` | string
`productId` | string
`services` | Array&lt;string&gt;
`additionalParameters` | [{ [key: string]: CreateShippingRuleRequestAdditionalParametersValue; }](CreateShippingRuleRequestAdditionalParametersValue.md)
`addressId` | string
`receivingCountries` | Array&lt;string&gt;
`emailNotification` | boolean
`phoneNotification` | boolean
`minWeight` | number
`maxWeight` | number
`minOrderValue` | number
`maxOrderValue` | number
`conditions` | [Array&lt;CreateShippingRuleRequestConditionsInner&gt;](CreateShippingRuleRequestConditionsInner.md)
`generateProformaInvoice` | boolean
`generateCommercialInvoice` | boolean
`generatePackingList` | boolean
`autoPrintLabels` | boolean
`autoPrintDocuments` | boolean
`labelPrinterId` | string
`documentPrinterId` | string
`returnShippingRuleId` | string
`autoCreateReturnShipment` | boolean
`brandId` | string

## Example

```typescript
import type { CreateShippingRuleRequest } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Standard DK,
  "description": Standard levering i Danmark,
  "direction": outbound,
  "carrierId": carr_01HZX9K2QF,
  "productId": PNL13,
  "services": ["EMAIL_NOTIFICATION"],
  "additionalParameters": {"returnFunctionality":"LABELLESS","returnQrEmail":true},
  "addressId": addr_01HZX9K2QF,
  "receivingCountries": ["DK","SE"],
  "emailNotification": true,
  "phoneNotification": false,
  "minWeight": 0,
  "maxWeight": 20,
  "minOrderValue": 0,
  "maxOrderValue": 5000,
  "conditions": [{"type":"flatRate","shippingPrice":39,"currency":"DKK"}],
  "generateProformaInvoice": false,
  "generateCommercialInvoice": false,
  "generatePackingList": false,
  "autoPrintLabels": false,
  "autoPrintDocuments": false,
  "labelPrinterId": null,
  "documentPrinterId": null,
  "returnShippingRuleId": null,
  "autoCreateReturnShipment": false,
  "brandId": brnd_8f3kd92ld0,
} satisfies CreateShippingRuleRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShippingRuleRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


