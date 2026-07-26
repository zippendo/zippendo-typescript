
# CreateShipment201ResponseShippingRule


## Properties

Name | Type
------------ | -------------
`id` | string
`name` | string
`carrierId` | string
`productId` | string
`services` | Array&lt;string&gt;
`addressId` | string
`returnShippingRuleId` | string
`autoCreateReturnShipment` | boolean
`autoPrintLabels` | boolean
`autoPrintDocuments` | boolean
`labelPrinterId` | string
`documentPrinterId` | string

## Example

```typescript
import type { CreateShipment201ResponseShippingRule } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": rule_3c4d5e6f,
  "name": Domestic standard,
  "carrierId": car_pn_001,
  "productId": prod_mypack_home,
  "services": ["A7"],
  "addressId": addr_7e8f9a0b,
  "returnShippingRuleId": rule_return_01,
  "autoCreateReturnShipment": false,
  "autoPrintLabels": true,
  "autoPrintDocuments": false,
  "labelPrinterId": prn_label_01,
  "documentPrinterId": prn_doc_01,
} satisfies CreateShipment201ResponseShippingRule

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShipment201ResponseShippingRule
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


