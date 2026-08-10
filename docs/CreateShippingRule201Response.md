
# CreateShippingRule201Response


## Properties

Name | Type
------------ | -------------
`id` | string
`name` | string
`description` | string
`direction` | string
`carrierId` | string
`productId` | string
`services` | Array&lt;string&gt;
`additionalParameters` | [{ [key: string]: ListShippingRules200ResponseDataInnerAdditionalParametersValue; }](ListShippingRules200ResponseDataInnerAdditionalParametersValue.md)
`addressId` | string
`receivingCountries` | Array&lt;string&gt;
`emailNotification` | boolean
`phoneNotification` | boolean
`minWeight` | number
`maxWeight` | number
`minOrderValue` | number
`maxOrderValue` | number
`conditions` | [Array&lt;ListShippingRules200ResponseDataInnerConditionsInner&gt;](ListShippingRules200ResponseDataInnerConditionsInner.md)
`generateProformaInvoice` | boolean
`generateCommercialInvoice` | boolean
`generatePackingList` | boolean
`autoPrintLabels` | boolean
`autoPrintDocuments` | boolean
`labelPrinterId` | string
`documentPrinterId` | string
`returnShippingRuleId` | string
`autoCreateReturnShipment` | boolean
`orgId` | string
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { CreateShippingRule201Response } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": rule_01HZX9K2QF,
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
  "orgId": org_01HZX9K2QF,
  "createdAt": 2026-06-22T09:00:00.000Z,
  "updatedAt": 2026-06-22T09:00:00.000Z,
} satisfies CreateShippingRule201Response

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShippingRule201Response
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


