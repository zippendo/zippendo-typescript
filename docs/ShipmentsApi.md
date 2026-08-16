# ShipmentsApi

All URIs are relative to *https://api.zippendo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**batchSendShipments**](ShipmentsApi.md#batchsendshipmentsoperation) | **POST** /orgs/{orgId}/shipments/batch-send | Batch send shipments |
| [**batchSplitShipment**](ShipmentsApi.md#batchsplitshipmentoperation) | **POST** /orgs/{orgId}/shipments/{shipmentId}/batch-split-shipment | Batch split shipment |
| [**createReturnShipment**](ShipmentsApi.md#createreturnshipment) | **POST** /orgs/{orgId}/shipments/{shipmentId}/create-return | Create return shipment |
| [**createShipment**](ShipmentsApi.md#createshipmentoperation) | **POST** /orgs/{orgId}/shipments | Create shipment |
| [**deleteShipment**](ShipmentsApi.md#deleteshipment) | **DELETE** /orgs/{orgId}/shipments/{shipmentId} | Delete shipment |
| [**getShipment**](ShipmentsApi.md#getshipment) | **GET** /orgs/{orgId}/shipments/{shipmentId} | Get shipment |
| [**getShipmentDocumentContent**](ShipmentsApi.md#getshipmentdocumentcontent) | **GET** /orgs/{orgId}/shipments/{shipmentId}/documents/{documentId}/content | Download shipment document |
| [**listShipments**](ShipmentsApi.md#listshipments) | **GET** /orgs/{orgId}/shipments | List shipments |
| [**sendShipment**](ShipmentsApi.md#sendshipment) | **POST** /orgs/{orgId}/shipments/{shipmentId}/send | Send shipment |
| [**splitShipment**](ShipmentsApi.md#splitshipmentoperation) | **POST** /orgs/{orgId}/shipments/{shipmentId}/split-shipment | Split shipment |
| [**splitShipmentParcel**](ShipmentsApi.md#splitshipmentparceloperation) | **POST** /orgs/{orgId}/shipments/{shipmentId}/split-parcel | Split parcels |
| [**trackShipment**](ShipmentsApi.md#trackshipment) | **GET** /orgs/{orgId}/shipments/{shipmentId}/tracking | Get shipment tracking |
| [**updateShipment**](ShipmentsApi.md#updateshipmentoperation) | **PATCH** /orgs/{orgId}/shipments/{shipmentId} | Update shipment |



## batchSendShipments

> BatchSendShipments200Response batchSendShipments(orgId, batchSendShipmentsRequest)

Batch send shipments

Book multiple pending/error shipments with their carriers in one request. Each shipment is processed independently and reported in &#x60;results&#x60;; a failure on one shipment never aborts the others. Use it to send every shipment on an order at once.

### Example

```ts
import {
  Configuration,
  ShipmentsApi,
} from '@zippendo/sdk';
import type { BatchSendShipmentsOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // BatchSendShipmentsRequest
    batchSendShipmentsRequest: ...,
  } satisfies BatchSendShipmentsOperationRequest;

  try {
    const data = await api.batchSendShipments(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orgId** | `string` | Organization ID | [Defaults to `undefined`] |
| **batchSendShipmentsRequest** | [BatchSendShipmentsRequest](BatchSendShipmentsRequest.md) |  | |

### Return type

[**BatchSendShipments200Response**](BatchSendShipments200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |
| **400** | Default Response |  -  |
| **403** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## batchSplitShipment

> BatchSplitShipment201Response batchSplitShipment(orgId, shipmentId, batchSplitShipmentRequest)

Batch split shipment

Split a parcel into multiple new shipments with per-line quantities in a single atomic operation. Only draft or pending shipments can be split.

### Example

```ts
import {
  Configuration,
  ShipmentsApi,
} from '@zippendo/sdk';
import type { BatchSplitShipmentOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentsApi(config);

  const body = {
    // string | Organization identifier.
    orgId: org_1a2b3c4d,
    // string | Shipment identifier.
    shipmentId: shp_4d9e7a2f,
    // BatchSplitShipmentRequest
    batchSplitShipmentRequest: ...,
  } satisfies BatchSplitShipmentOperationRequest;

  try {
    const data = await api.batchSplitShipment(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orgId** | `string` | Organization identifier. | [Defaults to `undefined`] |
| **shipmentId** | `string` | Shipment identifier. | [Defaults to `undefined`] |
| **batchSplitShipmentRequest** | [BatchSplitShipmentRequest](BatchSplitShipmentRequest.md) |  | |

### Return type

[**BatchSplitShipment201Response**](BatchSplitShipment201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Default Response |  -  |
| **400** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createReturnShipment

> CreateShipment201Response createReturnShipment(orgId, shipmentId)

Create return shipment

Create and auto-send a return shipment from a dispatched outbound shipment with swapped sender/receiver. Requires a configured return shipping rule.

### Example

```ts
import {
  Configuration,
  ShipmentsApi,
} from '@zippendo/sdk';
import type { CreateReturnShipmentRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentsApi(config);

  const body = {
    // string | Organization identifier.
    orgId: org_1a2b3c4d,
    // string | Shipment identifier.
    shipmentId: shp_4d9e7a2f,
  } satisfies CreateReturnShipmentRequest;

  try {
    const data = await api.createReturnShipment(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orgId** | `string` | Organization identifier. | [Defaults to `undefined`] |
| **shipmentId** | `string` | Shipment identifier. | [Defaults to `undefined`] |

### Return type

[**CreateShipment201Response**](CreateShipment201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |
| **400** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createShipment

> CreateShipment201Response createShipment(orgId, createShipmentRequest)

Create shipment

Create a new shipment for an organization. When orderId is provided, parties and parcels are derived from the order.

### Example

```ts
import {
  Configuration,
  ShipmentsApi,
} from '@zippendo/sdk';
import type { CreateShipmentOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // CreateShipmentRequest
    createShipmentRequest: ...,
  } satisfies CreateShipmentOperationRequest;

  try {
    const data = await api.createShipment(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orgId** | `string` | Organization ID | [Defaults to `undefined`] |
| **createShipmentRequest** | [CreateShipmentRequest](CreateShipmentRequest.md) |  | |

### Return type

[**CreateShipment201Response**](CreateShipment201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Default Response |  -  |
| **400** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteShipment

> RevokeApiToken200Response deleteShipment(orgId, shipmentId)

Delete shipment

Delete a shipment. Only shipments in pending status can be deleted.

### Example

```ts
import {
  Configuration,
  ShipmentsApi,
} from '@zippendo/sdk';
import type { DeleteShipmentRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentsApi(config);

  const body = {
    // string | Organization identifier.
    orgId: org_1a2b3c4d,
    // string | Shipment identifier.
    shipmentId: shp_4d9e7a2f,
  } satisfies DeleteShipmentRequest;

  try {
    const data = await api.deleteShipment(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orgId** | `string` | Organization identifier. | [Defaults to `undefined`] |
| **shipmentId** | `string` | Shipment identifier. | [Defaults to `undefined`] |

### Return type

[**RevokeApiToken200Response**](RevokeApiToken200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |
| **400** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getShipment

> CreateShipment201Response getShipment(orgId, shipmentId)

Get shipment

Retrieve a single shipment by its ID, including parcels, parties, documents and activity.

### Example

```ts
import {
  Configuration,
  ShipmentsApi,
} from '@zippendo/sdk';
import type { GetShipmentRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentsApi(config);

  const body = {
    // string | Organization identifier.
    orgId: org_1a2b3c4d,
    // string | Shipment identifier.
    shipmentId: shp_4d9e7a2f,
  } satisfies GetShipmentRequest;

  try {
    const data = await api.getShipment(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orgId** | `string` | Organization identifier. | [Defaults to `undefined`] |
| **shipmentId** | `string` | Shipment identifier. | [Defaults to `undefined`] |

### Return type

[**CreateShipment201Response**](CreateShipment201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getShipmentDocumentContent

> getShipmentDocumentContent(orgId, shipmentId, documentId, disposition, filename)

Download shipment document

Streams a shipment document or label file from storage.

### Example

```ts
import {
  Configuration,
  ShipmentsApi,
} from '@zippendo/sdk';
import type { GetShipmentDocumentContentRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentsApi(config);

  const body = {
    // string | Organization identifier.
    orgId: org_1a2b3c4d,
    // string | Shipment identifier.
    shipmentId: shp_4d9e7a2f,
    // string | Document identifier.
    documentId: doc_8f3a2b1c,
    // 'inline' | 'attachment' | Render the document inline (default) or force a download. (optional)
    disposition: inline,
    // string | Suggested filename (without extension) for attachment downloads. (optional)
    filename: label,
  } satisfies GetShipmentDocumentContentRequest;

  try {
    const data = await api.getShipmentDocumentContent(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orgId** | `string` | Organization identifier. | [Defaults to `undefined`] |
| **shipmentId** | `string` | Shipment identifier. | [Defaults to `undefined`] |
| **documentId** | `string` | Document identifier. | [Defaults to `undefined`] |
| **disposition** | `inline`, `attachment` | Render the document inline (default) or force a download. | [Optional] [Defaults to `&#39;inline&#39;`] [Enum: inline, attachment] |
| **filename** | `string` | Suggested filename (without extension) for attachment downloads. | [Optional] [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listShipments

> ListShipments200Response listShipments(orgId, page, limit, brandId, brandScope)

List shipments

List all shipments for an organization, paginated and ordered by newest first.

### Example

```ts
import {
  Configuration,
  ShipmentsApi,
} from '@zippendo/sdk';
import type { ListShipmentsRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // number | Page number (1-based) (optional)
    page: 1,
    // number | Items per page (max 100) (optional)
    limit: 20,
    // string | Filter by brand. Pass a brand ID, or \"none\" for records not assigned to any brand. (optional)
    brandId: brnd_8f3kd92ld0,
    // 'own' | 'shared' | 'both' | How the brand context narrows this list: \"own\" returns only rows assigned to the current brand (requires a brand session, a brand-bound token, or the X-Zippendo-Brand header), \"shared\" returns only unassigned organization-wide rows, \"both\" (default) returns both. The X-Zippendo-Brand-Scope header supplies a default when the parameter is omitted. For strictly brand-owned records (orders, shipments), a brand-scoped request combined with \"shared\" returns no rows, since those records are never visible organization-wide from within a brand context. (optional)
    brandScope: own,
  } satisfies ListShipmentsRequest;

  try {
    const data = await api.listShipments(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orgId** | `string` | Organization ID | [Defaults to `undefined`] |
| **page** | `number` | Page number (1-based) | [Optional] [Defaults to `1`] |
| **limit** | `number` | Items per page (max 100) | [Optional] [Defaults to `20`] |
| **brandId** | `string` | Filter by brand. Pass a brand ID, or \&quot;none\&quot; for records not assigned to any brand. | [Optional] [Defaults to `undefined`] |
| **brandScope** | `own`, `shared`, `both` | How the brand context narrows this list: \&quot;own\&quot; returns only rows assigned to the current brand (requires a brand session, a brand-bound token, or the X-Zippendo-Brand header), \&quot;shared\&quot; returns only unassigned organization-wide rows, \&quot;both\&quot; (default) returns both. The X-Zippendo-Brand-Scope header supplies a default when the parameter is omitted. For strictly brand-owned records (orders, shipments), a brand-scoped request combined with \&quot;shared\&quot; returns no rows, since those records are never visible organization-wide from within a brand context. | [Optional] [Defaults to `undefined`] [Enum: own, shared, both] |

### Return type

[**ListShipments200Response**](ListShipments200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |
| **400** | Default Response |  -  |
| **403** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## sendShipment

> CreateShipment201Response sendShipment(orgId, shipmentId)

Send shipment

Book a pending or error shipment with the carrier, generating labels and tracking. Returns 422 with carrier errors if booking fails.

### Example

```ts
import {
  Configuration,
  ShipmentsApi,
} from '@zippendo/sdk';
import type { SendShipmentRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentsApi(config);

  const body = {
    // string | Organization identifier.
    orgId: org_1a2b3c4d,
    // string | Shipment identifier.
    shipmentId: shp_4d9e7a2f,
  } satisfies SendShipmentRequest;

  try {
    const data = await api.sendShipment(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orgId** | `string` | Organization identifier. | [Defaults to `undefined`] |
| **shipmentId** | `string` | Shipment identifier. | [Defaults to `undefined`] |

### Return type

[**CreateShipment201Response**](CreateShipment201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |
| **400** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |
| **422** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## splitShipment

> SplitShipment201Response splitShipment(orgId, shipmentId, splitShipmentRequest)

Split shipment

Move order lines from a parcel into a new shipment. Only draft or pending shipments can be split.

### Example

```ts
import {
  Configuration,
  ShipmentsApi,
} from '@zippendo/sdk';
import type { SplitShipmentOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentsApi(config);

  const body = {
    // string | Organization identifier.
    orgId: org_1a2b3c4d,
    // string | Shipment identifier.
    shipmentId: shp_4d9e7a2f,
    // SplitShipmentRequest
    splitShipmentRequest: ...,
  } satisfies SplitShipmentOperationRequest;

  try {
    const data = await api.splitShipment(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orgId** | `string` | Organization identifier. | [Defaults to `undefined`] |
| **shipmentId** | `string` | Shipment identifier. | [Defaults to `undefined`] |
| **splitShipmentRequest** | [SplitShipmentRequest](SplitShipmentRequest.md) |  | |

### Return type

[**SplitShipment201Response**](SplitShipment201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Default Response |  -  |
| **400** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## splitShipmentParcel

> SplitShipmentParcel200Response splitShipmentParcel(orgId, shipmentId, splitShipmentParcelRequest)

Split parcels

Redistribute order lines across parcels within a shipment, moving lines between parcels and creating new ones. Only draft, pending or error shipments can be modified.

### Example

```ts
import {
  Configuration,
  ShipmentsApi,
} from '@zippendo/sdk';
import type { SplitShipmentParcelOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentsApi(config);

  const body = {
    // string | Organization identifier.
    orgId: org_1a2b3c4d,
    // string | Shipment identifier.
    shipmentId: shp_4d9e7a2f,
    // SplitShipmentParcelRequest
    splitShipmentParcelRequest: ...,
  } satisfies SplitShipmentParcelOperationRequest;

  try {
    const data = await api.splitShipmentParcel(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orgId** | `string` | Organization identifier. | [Defaults to `undefined`] |
| **shipmentId** | `string` | Shipment identifier. | [Defaults to `undefined`] |
| **splitShipmentParcelRequest** | [SplitShipmentParcelRequest](SplitShipmentParcelRequest.md) |  | |

### Return type

[**SplitShipmentParcel200Response**](SplitShipmentParcel200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |
| **400** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## trackShipment

> TrackShipment200Response trackShipment(orgId, shipmentId)

Get shipment tracking

Retrieve the tracking timeline for a shipment, including current status and all carrier events.

### Example

```ts
import {
  Configuration,
  ShipmentsApi,
} from '@zippendo/sdk';
import type { TrackShipmentRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentsApi(config);

  const body = {
    // string | Organization identifier.
    orgId: org_1a2b3c4d,
    // string | Shipment identifier.
    shipmentId: shp_4d9e7a2f,
  } satisfies TrackShipmentRequest;

  try {
    const data = await api.trackShipment(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orgId** | `string` | Organization identifier. | [Defaults to `undefined`] |
| **shipmentId** | `string` | Shipment identifier. | [Defaults to `undefined`] |

### Return type

[**TrackShipment200Response**](TrackShipment200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateShipment

> CreateShipment201Response updateShipment(orgId, shipmentId, updateShipmentRequest)

Update shipment

Update an existing shipment. Only draft, pending or error shipments can be updated; an applied shipping rule overrides carrier settings and sender party.

### Example

```ts
import {
  Configuration,
  ShipmentsApi,
} from '@zippendo/sdk';
import type { UpdateShipmentOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentsApi(config);

  const body = {
    // string | Organization identifier.
    orgId: org_1a2b3c4d,
    // string | Shipment identifier.
    shipmentId: shp_4d9e7a2f,
    // UpdateShipmentRequest
    updateShipmentRequest: ...,
  } satisfies UpdateShipmentOperationRequest;

  try {
    const data = await api.updateShipment(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orgId** | `string` | Organization identifier. | [Defaults to `undefined`] |
| **shipmentId** | `string` | Shipment identifier. | [Defaults to `undefined`] |
| **updateShipmentRequest** | [UpdateShipmentRequest](UpdateShipmentRequest.md) |  | |

### Return type

[**CreateShipment201Response**](CreateShipment201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |
| **400** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

