
# HealthCheck200Response


## Properties

Name | Type
------------ | -------------
`status` | string
`timestamp` | string
`version` | string

## Example

```typescript
import type { HealthCheck200Response } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "status": ok,
  "timestamp": 2026-06-22T14:30:00.000Z,
  "version": 1.0.0,
} satisfies HealthCheck200Response

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as HealthCheck200Response
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


