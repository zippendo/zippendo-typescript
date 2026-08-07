# OrdersApi

All URIs are relative to *https://api.zippendo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createOrder**](OrdersApi.md#createorderoperation) | **POST** /orgs/{orgId}/orders | Create order |
| [**deleteOrder**](OrdersApi.md#deleteorder) | **DELETE** /orgs/{orgId}/orders/{orderId} | Delete order |
| [**getOrder**](OrdersApi.md#getorder) | **GET** /orgs/{orgId}/orders/{orderId} | Get order |
| [**listOrders**](OrdersApi.md#listorders) | **GET** /orgs/{orgId}/orders | List orders |
| [**updateOrder**](OrdersApi.md#updateorderoperation) | **PATCH** /orgs/{orgId}/orders/{orderId} | Update order |



## createOrder

> CreateOrder201Response createOrder(orgId, createOrderRequest)

Create order

Creates a new order under an existing order channel for the organization.

### Example

```ts
import {
  Configuration,
  OrdersApi,
} from '@zippendo/sdk';
import type { CreateOrderOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrdersApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // CreateOrderRequest
    createOrderRequest: ...,
  } satisfies CreateOrderOperationRequest;

  try {
    const data = await api.createOrder(body);
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
| **createOrderRequest** | [CreateOrderRequest](CreateOrderRequest.md) |  | |

### Return type

[**CreateOrder201Response**](CreateOrder201Response.md)

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


## deleteOrder

> RevokeApiToken200Response deleteOrder(orgId, orderId)

Delete order

Deletes an order. Fails if the order has associated shipments.

### Example

```ts
import {
  Configuration,
  OrdersApi,
} from '@zippendo/sdk';
import type { DeleteOrderRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrdersApi(config);

  const body = {
    // string | Organization ID.
    orgId: clz9k2f0a0000abcd0000zzzz,
    // string | Order ID.
    orderId: clz9k2f0a0003abcd9012mnop,
  } satisfies DeleteOrderRequest;

  try {
    const data = await api.deleteOrder(body);
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
| **orgId** | `string` | Organization ID. | [Defaults to `undefined`] |
| **orderId** | `string` | Order ID. | [Defaults to `undefined`] |

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


## getOrder

> GetOrder200Response getOrder(orgId, orderId)

Get order

Returns a single order with its channel, shipping rule, shipments, and documents.

### Example

```ts
import {
  Configuration,
  OrdersApi,
} from '@zippendo/sdk';
import type { GetOrderRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrdersApi(config);

  const body = {
    // string | Organization ID.
    orgId: clz9k2f0a0000abcd0000zzzz,
    // string | Order ID.
    orderId: clz9k2f0a0003abcd9012mnop,
  } satisfies GetOrderRequest;

  try {
    const data = await api.getOrder(body);
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
| **orgId** | `string` | Organization ID. | [Defaults to `undefined`] |
| **orderId** | `string` | Order ID. | [Defaults to `undefined`] |

### Return type

[**GetOrder200Response**](GetOrder200Response.md)

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


## listOrders

> ListOrders200Response listOrders(orgId, page, limit, brandId, status, orderChannelId, search)

List orders

Returns a paginated list of orders for an organization, filterable by status, channel, and search term.

### Example

```ts
import {
  Configuration,
  OrdersApi,
} from '@zippendo/sdk';
import type { ListOrdersRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrdersApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // number | Page number (1-based) (optional)
    page: 1,
    // number | Items per page (max 100) (optional)
    limit: 20,
    // string | Filter by brand. Pass a brand ID, or \"none\" for records not assigned to any brand. (optional)
    brandId: brnd_8f3kd92ld0,
    // 'pending' | 'processing' | 'partially_fulfilled' | 'fulfilled' | 'error' | 'cancelled' | Order fulfilment status derived from its shipments. (optional)
    status: processing,
    // string | Filter by order channel ID. (optional)
    orderChannelId: clz9k2f0a0001abcd1234efgh,
    // string | Search by order number or customer name/email. (optional)
    search: Anna,
  } satisfies ListOrdersRequest;

  try {
    const data = await api.listOrders(body);
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
| **status** | `pending`, `processing`, `partially_fulfilled`, `fulfilled`, `error`, `cancelled` | Order fulfilment status derived from its shipments. | [Optional] [Defaults to `undefined`] [Enum: pending, processing, partially_fulfilled, fulfilled, error, cancelled] |
| **orderChannelId** | `string` | Filter by order channel ID. | [Optional] [Defaults to `undefined`] |
| **search** | `string` | Search by order number or customer name/email. | [Optional] [Defaults to `undefined`] |

### Return type

[**ListOrders200Response**](ListOrders200Response.md)

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


## updateOrder

> CreateOrder201Response updateOrder(orgId, orderId, updateOrderRequest)

Update order

Updates an order that is not yet fulfilled or cancelled.

### Example

```ts
import {
  Configuration,
  OrdersApi,
} from '@zippendo/sdk';
import type { UpdateOrderOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrdersApi(config);

  const body = {
    // string | Organization ID.
    orgId: clz9k2f0a0000abcd0000zzzz,
    // string | Order ID.
    orderId: clz9k2f0a0003abcd9012mnop,
    // UpdateOrderRequest
    updateOrderRequest: ...,
  } satisfies UpdateOrderOperationRequest;

  try {
    const data = await api.updateOrder(body);
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
| **orgId** | `string` | Organization ID. | [Defaults to `undefined`] |
| **orderId** | `string` | Order ID. | [Defaults to `undefined`] |
| **updateOrderRequest** | [UpdateOrderRequest](UpdateOrderRequest.md) |  | |

### Return type

[**CreateOrder201Response**](CreateOrder201Response.md)

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

