
# GetBillingUsage200ResponseLimits


## Properties

Name | Type
------------ | -------------
`teamMembers` | [GetBillingUsage200ResponseLimitsTeamMembers](GetBillingUsage200ResponseLimitsTeamMembers.md)
`carriers` | [GetBillingUsage200ResponseLimitsTeamMembers](GetBillingUsage200ResponseLimitsTeamMembers.md)
`orderChannels` | [GetBillingUsage200ResponseLimitsTeamMembers](GetBillingUsage200ResponseLimitsTeamMembers.md)
`shippingRules` | [GetBillingUsage200ResponseLimitsTeamMembers](GetBillingUsage200ResponseLimitsTeamMembers.md)
`addresses` | [GetBillingUsage200ResponseLimitsTeamMembers](GetBillingUsage200ResponseLimitsTeamMembers.md)
`apiTokens` | [GetBillingUsage200ResponseLimitsTeamMembers](GetBillingUsage200ResponseLimitsTeamMembers.md)
`automations` | [GetBillingUsage200ResponseLimitsTeamMembers](GetBillingUsage200ResponseLimitsTeamMembers.md)

## Example

```typescript
import type { GetBillingUsage200ResponseLimits } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "teamMembers": null,
  "carriers": null,
  "orderChannels": null,
  "shippingRules": null,
  "addresses": null,
  "apiTokens": null,
  "automations": null,
} satisfies GetBillingUsage200ResponseLimits

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GetBillingUsage200ResponseLimits
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


