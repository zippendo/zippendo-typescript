# CarriersApi

All URIs are relative to *https://api.zippendo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**connectCarrier**](CarriersApi.md#connectcarrieroperation) | **POST** /orgs/{orgId}/carriers | Connect carrier |
| [**disconnectCarrier**](CarriersApi.md#disconnectcarrier) | **DELETE** /orgs/{orgId}/carriers/{carrierId} | Disconnect carrier |
| [**getCarrier**](CarriersApi.md#getcarrier) | **GET** /orgs/{orgId}/carriers/{carrierId} | Get carrier |
| [**listCarrierProductServicePoints**](CarriersApi.md#listcarrierproductservicepointsoperation) | **POST** /orgs/{orgId}/carriers/{carrierId}/products/{productId}/service-points | List product service points |
| [**listCarrierProducts**](CarriersApi.md#listcarrierproducts) | **GET** /orgs/{orgId}/carriers/{carrierId}/products | List carrier products |
| [**listCarriers**](CarriersApi.md#listcarriers) | **GET** /orgs/{orgId}/carriers | List carriers |
| [**updateCarrier**](CarriersApi.md#updatecarrieroperation) | **PUT** /orgs/{orgId}/carriers/{carrierId} | Update carrier |



## connectCarrier

> ListCarriers200ResponseDataInner connectCarrier(orgId, connectCarrierRequest)

Connect carrier

Connects a new carrier to the organization with its configuration.

### Example

```ts
import {
  Configuration,
  CarriersApi,
} from '@zippendo/sdk';
import type { ConnectCarrierOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CarriersApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
    // ConnectCarrierRequest
    connectCarrierRequest: ...,
  } satisfies ConnectCarrierOperationRequest;

  try {
    const data = await api.connectCarrier(body);
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
| **connectCarrierRequest** | [ConnectCarrierRequest](ConnectCarrierRequest.md) |  | |

### Return type

[**ListCarriers200ResponseDataInner**](ListCarriers200ResponseDataInner.md)

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


## disconnectCarrier

> string disconnectCarrier(orgId, carrierId)

Disconnect carrier

Disconnects a carrier from the organization.

### Example

```ts
import {
  Configuration,
  CarriersApi,
} from '@zippendo/sdk';
import type { DisconnectCarrierRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CarriersApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
    // string | Carrier ID
    carrierId: carr_01HZX9K2QF,
  } satisfies DisconnectCarrierRequest;

  try {
    const data = await api.disconnectCarrier(body);
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
| **carrierId** | `string` | Carrier ID | [Defaults to `undefined`] |

### Return type

**string**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getCarrier

> ListCarriers200ResponseDataInner getCarrier(orgId, carrierId)

Get carrier

Returns a single connected carrier.

### Example

```ts
import {
  Configuration,
  CarriersApi,
} from '@zippendo/sdk';
import type { GetCarrierRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CarriersApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
    // string | Carrier ID
    carrierId: carr_01HZX9K2QF,
  } satisfies GetCarrierRequest;

  try {
    const data = await api.getCarrier(body);
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
| **carrierId** | `string` | Carrier ID | [Defaults to `undefined`] |

### Return type

[**ListCarriers200ResponseDataInner**](ListCarriers200ResponseDataInner.md)

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


## listCarrierProductServicePoints

> Array&lt;ListCarrierProductServicePoints200ResponseInner&gt; listCarrierProductServicePoints(orgId, carrierId, productId, listCarrierProductServicePointsRequest)

List product service points

Returns pickup service points near a location for a specific carrier product.

### Example

```ts
import {
  Configuration,
  CarriersApi,
} from '@zippendo/sdk';
import type { ListCarrierProductServicePointsOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CarriersApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
    // string | Carrier ID
    carrierId: carr_01HZX9K2QF,
    // string | Carrier product ID
    productId: PNL13,
    // ListCarrierProductServicePointsRequest
    listCarrierProductServicePointsRequest: ...,
  } satisfies ListCarrierProductServicePointsOperationRequest;

  try {
    const data = await api.listCarrierProductServicePoints(body);
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
| **carrierId** | `string` | Carrier ID | [Defaults to `undefined`] |
| **productId** | `string` | Carrier product ID | [Defaults to `undefined`] |
| **listCarrierProductServicePointsRequest** | [ListCarrierProductServicePointsRequest](ListCarrierProductServicePointsRequest.md) |  | |

### Return type

[**Array&lt;ListCarrierProductServicePoints200ResponseInner&gt;**](ListCarrierProductServicePoints200ResponseInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listCarrierProducts

> Array&lt;ListCarrierProducts200ResponseInner&gt; listCarrierProducts(orgId, carrierId)

List carrier products

Returns the shipping products available for a connected carrier.

### Example

```ts
import {
  Configuration,
  CarriersApi,
} from '@zippendo/sdk';
import type { ListCarrierProductsRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CarriersApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
    // string | Carrier ID
    carrierId: carr_01HZX9K2QF,
  } satisfies ListCarrierProductsRequest;

  try {
    const data = await api.listCarrierProducts(body);
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
| **carrierId** | `string` | Carrier ID | [Defaults to `undefined`] |

### Return type

[**Array&lt;ListCarrierProducts200ResponseInner&gt;**](ListCarrierProducts200ResponseInner.md)

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


## listCarriers

> ListCarriers200Response listCarriers(orgId, page, limit, brandId, brandScope)

List carriers

Returns a paginated list of carriers connected to the organization.

### Example

```ts
import {
  Configuration,
  CarriersApi,
} from '@zippendo/sdk';
import type { ListCarriersRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CarriersApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
    // number | Page number (1-based) (optional)
    page: 1,
    // number | Items per page (max 100) (optional)
    limit: 20,
    // string | Filter by brand. Pass a brand ID, or \"none\" for records not assigned to any brand. (optional)
    brandId: brnd_8f3kd92ld0,
    // 'own' | 'shared' | 'both' | How the brand context narrows this list: \"own\" returns only rows assigned to the current brand (requires a brand session, a brand-bound token, or the X-Zippendo-Brand header), \"shared\" returns only unassigned organization-wide rows, \"both\" (default) returns both. The X-Zippendo-Brand-Scope header supplies a default when the parameter is omitted. For strictly brand-owned records (orders, shipments), a brand-scoped request combined with \"shared\" returns no rows, since those records are never visible organization-wide from within a brand context. (optional)
    brandScope: own,
  } satisfies ListCarriersRequest;

  try {
    const data = await api.listCarriers(body);
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

[**ListCarriers200Response**](ListCarriers200Response.md)

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

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateCarrier

> ListCarriers200ResponseDataInner updateCarrier(orgId, carrierId, updateCarrierRequest)

Update carrier

Updates a connected carrier\&#39;s configuration or name.

### Example

```ts
import {
  Configuration,
  CarriersApi,
} from '@zippendo/sdk';
import type { UpdateCarrierOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CarriersApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
    // string | Carrier ID
    carrierId: carr_01HZX9K2QF,
    // UpdateCarrierRequest
    updateCarrierRequest: ...,
  } satisfies UpdateCarrierOperationRequest;

  try {
    const data = await api.updateCarrier(body);
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
| **carrierId** | `string` | Carrier ID | [Defaults to `undefined`] |
| **updateCarrierRequest** | [UpdateCarrierRequest](UpdateCarrierRequest.md) |  | |

### Return type

[**ListCarriers200ResponseDataInner**](ListCarriers200ResponseDataInner.md)

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

