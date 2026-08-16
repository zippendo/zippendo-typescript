
# GetBillingUsage200ResponseZippyMessages

Zippy AI message usage this period (present when Zippy access is enabled)

## Properties

Name | Type
------------ | -------------
`used` | number
`charges` | number

## Example

```typescript
import type { GetBillingUsage200ResponseZippyMessages } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "used": 42,
  "charges": 4158,
} satisfies GetBillingUsage200ResponseZippyMessages

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GetBillingUsage200ResponseZippyMessages
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


