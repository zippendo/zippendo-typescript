
# CreateShipment201ResponseTracking


## Properties

Name | Type
------------ | -------------
`url` | string
`number` | string
`labelFreeCode` | string
`qrCodeLink` | string
`qrCodeDataUri` | string
`qrCodeUrl` | string

## Example

```typescript
import type { CreateShipment201ResponseTracking } from '@zippendo/sdk'

// TODO: Update the object below with actual values
const example = {
  "url": https://tracking.postnord.com/00370724710000012345,
  "number": 00370724710000012345,
  "labelFreeCode": AB12CD34,
  "qrCodeLink": data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNk+M9QDwADhgGAWjR9awAAAABJRU5ErkJggg==,
  "qrCodeDataUri": data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNk+M9QDwADhgGAWjR9awAAAABJRU5ErkJggg==,
  "qrCodeUrl": https://qr.bring.com/label-free/AB12CD34.png,
} satisfies CreateShipment201ResponseTracking

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShipment201ResponseTracking
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


