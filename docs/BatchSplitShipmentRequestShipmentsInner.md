
# BatchSplitShipmentRequestShipmentsInner


## Properties

Name | Type
------------ | -------------
`reference` | string
`orderLines` | [Array&lt;BatchSplitShipmentRequestShipmentsInnerOrderLinesInner&gt;](BatchSplitShipmentRequestShipmentsInnerOrderLinesInner.md)

## Example

```typescript
import type { BatchSplitShipmentRequestShipmentsInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "reference": ORDER-1042-split-1,
  "orderLines": null,
} satisfies BatchSplitShipmentRequestShipmentsInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BatchSplitShipmentRequestShipmentsInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


