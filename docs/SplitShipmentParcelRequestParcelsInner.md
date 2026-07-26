
# SplitShipmentParcelRequestParcelsInner


## Properties

Name | Type
------------ | -------------
`id` | string
`orderLines` | [Array&lt;BatchSplitShipmentRequestShipmentsInnerOrderLinesInner&gt;](BatchSplitShipmentRequestShipmentsInnerOrderLinesInner.md)

## Example

```typescript
import type { SplitShipmentParcelRequestParcelsInner } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": prc_5a6b7c8d,
  "orderLines": null,
} satisfies SplitShipmentParcelRequestParcelsInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SplitShipmentParcelRequestParcelsInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


