
# ListOrders200ResponseDataInnerOrderChannel

Summary of the order\'s source channel.

## Properties

Name | Type
------------ | -------------
`id` | string
`name` | string
`type` | string

## Example

```typescript
import type { ListOrders200ResponseDataInnerOrderChannel } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": clz9k2f0a0001abcd1234efgh,
  "name": Anna's Shopify Store,
  "type": shopify,
} satisfies ListOrders200ResponseDataInnerOrderChannel

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListOrders200ResponseDataInnerOrderChannel
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


