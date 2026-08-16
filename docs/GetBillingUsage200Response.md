
# GetBillingUsage200Response


## Properties

Name | Type
------------ | -------------
`currentPeriod` | [GetBillingUsage200ResponseCurrentPeriod](GetBillingUsage200ResponseCurrentPeriod.md)
`shipments` | [GetBillingUsage200ResponseShipments](GetBillingUsage200ResponseShipments.md)
`limits` | [GetBillingUsage200ResponseLimits](GetBillingUsage200ResponseLimits.md)
`addOns` | [Array&lt;GetBillingUsage200ResponseAddOnsInner&gt;](GetBillingUsage200ResponseAddOnsInner.md)
`zippyMessages` | [GetBillingUsage200ResponseZippyMessages](GetBillingUsage200ResponseZippyMessages.md)

## Example

```typescript
import type { GetBillingUsage200Response } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "currentPeriod": null,
  "shipments": null,
  "limits": null,
  "addOns": [],
  "zippyMessages": null,
} satisfies GetBillingUsage200Response

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GetBillingUsage200Response
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


