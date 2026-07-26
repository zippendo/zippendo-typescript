
# CreateShippingQuote200ResponseRatesInner


## Properties

Name | Type
------------ | -------------
`serviceName` | string
`serviceCode` | string
`totalPrice` | string
`currency` | string
`description` | string
`minDeliveryDate` | string
`maxDeliveryDate` | string
`carrierName` | string
`carrierSlug` | string
`productId` | string
`shippingRuleId` | string

## Example

```typescript
import type { CreateShippingQuote200ResponseRatesInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "serviceName": Standard DK,
  "serviceCode": postnord:PNL13:rule_01HZX9K2QF,
  "totalPrice": 3900,
  "currency": DKK,
  "description": Standard levering i Danmark,
  "minDeliveryDate": 2026-06-24,
  "maxDeliveryDate": 2026-06-26,
  "carrierName": PostNord,
  "carrierSlug": postnord,
  "productId": PNL13,
  "shippingRuleId": rule_01HZX9K2QF,
} satisfies CreateShippingQuote200ResponseRatesInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShippingQuote200ResponseRatesInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


