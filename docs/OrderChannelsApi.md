# OrderChannelsApi

All URIs are relative to *https://api.zippendo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createOrderChannel**](OrderChannelsApi.md#createorderchanneloperation) | **POST** /orgs/{orgId}/order-channels | Create order channel |
| [**createOrderChannelWebhookSecret**](OrderChannelsApi.md#createorderchannelwebhooksecret) | **POST** /orgs/{orgId}/order-channels/{channelId}/webhook-secret | Create or rotate webhook signing secret |
| [**deleteOrderChannel**](OrderChannelsApi.md#deleteorderchannel) | **DELETE** /orgs/{orgId}/order-channels/{channelId} | Delete order channel |
| [**getOrderChannel**](OrderChannelsApi.md#getorderchannel) | **GET** /orgs/{orgId}/order-channels/{channelId} | Get order channel |
| [**getOrderChannelWebhookStatus**](OrderChannelsApi.md#getorderchannelwebhookstatus) | **GET** /orgs/{orgId}/order-channels/{channelId}/webhooks | Get channel webhook status |
| [**listOrderChannels**](OrderChannelsApi.md#listorderchannels) | **GET** /orgs/{orgId}/order-channels | List order channels |
| [**revokeOrderChannelWebhookSecret**](OrderChannelsApi.md#revokeorderchannelwebhooksecret) | **DELETE** /orgs/{orgId}/order-channels/{channelId}/webhook-secret | Revoke webhook signing secret |
| [**updateOrderChannel**](OrderChannelsApi.md#updateorderchanneloperation) | **PATCH** /orgs/{orgId}/order-channels/{channelId} | Update order channel |



## createOrderChannel

> ListOrderChannels200ResponseDataInner createOrderChannel(orgId, createOrderChannelRequest)

Create order channel

Creates a new order channel for an organization.

### Example

```ts
import {
  Configuration,
  OrderChannelsApi,
} from '@zippendo/sdk';
import type { CreateOrderChannelOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderChannelsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // CreateOrderChannelRequest
    createOrderChannelRequest: ...,
  } satisfies CreateOrderChannelOperationRequest;

  try {
    const data = await api.createOrderChannel(body);
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
| **createOrderChannelRequest** | [CreateOrderChannelRequest](CreateOrderChannelRequest.md) |  | |

### Return type

[**ListOrderChannels200ResponseDataInner**](ListOrderChannels200ResponseDataInner.md)

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

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createOrderChannelWebhookSecret

> CreateOrderChannelWebhookSecret201Response createOrderChannelWebhookSecret(orgId, channelId)

Create or rotate webhook signing secret

Generates (or rotates) the custom channel\&#39;s webhook signing secret used to authenticate order pushes to the ingest URL. The secret is returned only once. Rotating invalidates the previous secret immediately.

### Example

```ts
import {
  Configuration,
  OrderChannelsApi,
} from '@zippendo/sdk';
import type { CreateOrderChannelWebhookSecretRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderChannelsApi(config);

  const body = {
    // string | Organization ID.
    orgId: clz9k2f0a0000abcd0000zzzz,
    // string | Order channel ID.
    channelId: clz9k2f0a0001abcd1234efgh,
  } satisfies CreateOrderChannelWebhookSecretRequest;

  try {
    const data = await api.createOrderChannelWebhookSecret(body);
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
| **channelId** | `string` | Order channel ID. | [Defaults to `undefined`] |

### Return type

[**CreateOrderChannelWebhookSecret201Response**](CreateOrderChannelWebhookSecret201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Default Response |  -  |
| **400** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteOrderChannel

> RevokeApiToken200Response deleteOrderChannel(orgId, channelId)

Delete order channel

Deletes an order channel and cascades deletion of its orders.

### Example

```ts
import {
  Configuration,
  OrderChannelsApi,
} from '@zippendo/sdk';
import type { DeleteOrderChannelRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderChannelsApi(config);

  const body = {
    // string | Organization ID.
    orgId: clz9k2f0a0000abcd0000zzzz,
    // string | Order channel ID.
    channelId: clz9k2f0a0001abcd1234efgh,
  } satisfies DeleteOrderChannelRequest;

  try {
    const data = await api.deleteOrderChannel(body);
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
| **channelId** | `string` | Order channel ID. | [Defaults to `undefined`] |

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


## getOrderChannel

> ListOrderChannels200ResponseDataInner getOrderChannel(orgId, channelId)

Get order channel

Returns a single order channel by ID, including its linked shipping rules.

### Example

```ts
import {
  Configuration,
  OrderChannelsApi,
} from '@zippendo/sdk';
import type { GetOrderChannelRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderChannelsApi(config);

  const body = {
    // string | Organization ID.
    orgId: clz9k2f0a0000abcd0000zzzz,
    // string | Order channel ID.
    channelId: clz9k2f0a0001abcd1234efgh,
  } satisfies GetOrderChannelRequest;

  try {
    const data = await api.getOrderChannel(body);
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
| **channelId** | `string` | Order channel ID. | [Defaults to `undefined`] |

### Return type

[**ListOrderChannels200ResponseDataInner**](ListOrderChannels200ResponseDataInner.md)

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


## getOrderChannelWebhookStatus

> GetOrderChannelWebhookStatus200Response getOrderChannelWebhookStatus(orgId, channelId)

Get channel webhook status

Returns whether webhooks are enabled and lists the webhooks registered with the platform.

### Example

```ts
import {
  Configuration,
  OrderChannelsApi,
} from '@zippendo/sdk';
import type { GetOrderChannelWebhookStatusRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderChannelsApi(config);

  const body = {
    // string | Organization ID.
    orgId: clz9k2f0a0000abcd0000zzzz,
    // string | Order channel ID.
    channelId: clz9k2f0a0001abcd1234efgh,
  } satisfies GetOrderChannelWebhookStatusRequest;

  try {
    const data = await api.getOrderChannelWebhookStatus(body);
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
| **channelId** | `string` | Order channel ID. | [Defaults to `undefined`] |

### Return type

[**GetOrderChannelWebhookStatus200Response**](GetOrderChannelWebhookStatus200Response.md)

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


## listOrderChannels

> ListOrderChannels200Response listOrderChannels(orgId, page, limit, brandId, brandScope, type, enabled, search)

List order channels

Returns a paginated list of order channels for an organization.

### Example

```ts
import {
  Configuration,
  OrderChannelsApi,
} from '@zippendo/sdk';
import type { ListOrderChannelsRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderChannelsApi(config);

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
    // 'shopify' | 'woocommerce' | 'manual' | 'custom' | Filter by channel type. (optional)
    type: shopify,
    // string | Filter by enabled state. (optional)
    enabled: true,
    // string | Search by channel name. (optional)
    search: Anna's Shopify Store,
  } satisfies ListOrderChannelsRequest;

  try {
    const data = await api.listOrderChannels(body);
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
| **type** | `shopify`, `woocommerce`, `manual`, `custom` | Filter by channel type. | [Optional] [Defaults to `undefined`] [Enum: shopify, woocommerce, manual, custom] |
| **enabled** | `string` | Filter by enabled state. | [Optional] [Defaults to `undefined`] |
| **search** | `string` | Search by channel name. | [Optional] [Defaults to `undefined`] |

### Return type

[**ListOrderChannels200Response**](ListOrderChannels200Response.md)

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


## revokeOrderChannelWebhookSecret

> RevokeOrderChannelWebhookSecret200Response revokeOrderChannelWebhookSecret(orgId, channelId)

Revoke webhook signing secret

Revokes the custom channel\&#39;s webhook signing secret. All subsequent pushes to the ingest URL are rejected until a new secret is generated.

### Example

```ts
import {
  Configuration,
  OrderChannelsApi,
} from '@zippendo/sdk';
import type { RevokeOrderChannelWebhookSecretRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderChannelsApi(config);

  const body = {
    // string | Organization ID.
    orgId: clz9k2f0a0000abcd0000zzzz,
    // string | Order channel ID.
    channelId: clz9k2f0a0001abcd1234efgh,
  } satisfies RevokeOrderChannelWebhookSecretRequest;

  try {
    const data = await api.revokeOrderChannelWebhookSecret(body);
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
| **channelId** | `string` | Order channel ID. | [Defaults to `undefined`] |

### Return type

[**RevokeOrderChannelWebhookSecret200Response**](RevokeOrderChannelWebhookSecret200Response.md)

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


## updateOrderChannel

> ListOrderChannels200ResponseDataInner updateOrderChannel(orgId, channelId, updateOrderChannelRequest)

Update order channel

Updates an order channel and its linked shipping rules.

### Example

```ts
import {
  Configuration,
  OrderChannelsApi,
} from '@zippendo/sdk';
import type { UpdateOrderChannelOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderChannelsApi(config);

  const body = {
    // string | Organization ID.
    orgId: clz9k2f0a0000abcd0000zzzz,
    // string | Order channel ID.
    channelId: clz9k2f0a0001abcd1234efgh,
    // UpdateOrderChannelRequest
    updateOrderChannelRequest: ...,
  } satisfies UpdateOrderChannelOperationRequest;

  try {
    const data = await api.updateOrderChannel(body);
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
| **channelId** | `string` | Order channel ID. | [Defaults to `undefined`] |
| **updateOrderChannelRequest** | [UpdateOrderChannelRequest](UpdateOrderChannelRequest.md) |  | |

### Return type

[**ListOrderChannels200ResponseDataInner**](ListOrderChannels200ResponseDataInner.md)

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

