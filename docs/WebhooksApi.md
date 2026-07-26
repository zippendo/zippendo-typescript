# WebhooksApi

All URIs are relative to *https://api.zippendo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createOrgWebhook**](WebhooksApi.md#createorgwebhookoperation) | **POST** /orgs/{orgId}/webhooks | Create webhook |
| [**deleteOrgWebhook**](WebhooksApi.md#deleteorgwebhook) | **DELETE** /orgs/{orgId}/webhooks/{webhookId} | Delete webhook |
| [**getOrgWebhook**](WebhooksApi.md#getorgwebhook) | **GET** /orgs/{orgId}/webhooks/{webhookId} | Get webhook |
| [**listOrgWebhookDeliveries**](WebhooksApi.md#listorgwebhookdeliveries) | **GET** /orgs/{orgId}/webhooks/{webhookId}/deliveries | List webhook deliveries |
| [**listOrgWebhooks**](WebhooksApi.md#listorgwebhooks) | **GET** /orgs/{orgId}/webhooks | List webhooks |
| [**testOrgWebhook**](WebhooksApi.md#testorgwebhook) | **POST** /orgs/{orgId}/webhooks/{webhookId}/test | Test webhook |
| [**updateOrgWebhook**](WebhooksApi.md#updateorgwebhookoperation) | **PATCH** /orgs/{orgId}/webhooks/{webhookId} | Update webhook |



## createOrgWebhook

> CreateOrgWebhook201Response createOrgWebhook(orgId, createOrgWebhookRequest)

Create webhook

Create a new webhook endpoint for an organization that receives event notifications.

### Example

```ts
import {
  Configuration,
  WebhooksApi,
} from '@zippendo/sdk';
import type { CreateOrgWebhookOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WebhooksApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // CreateOrgWebhookRequest
    createOrgWebhookRequest: ...,
  } satisfies CreateOrgWebhookOperationRequest;

  try {
    const data = await api.createOrgWebhook(body);
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
| **createOrgWebhookRequest** | [CreateOrgWebhookRequest](CreateOrgWebhookRequest.md) |  | |

### Return type

[**CreateOrgWebhook201Response**](CreateOrgWebhook201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Default Response |  -  |
| **401** | Default Response |  -  |
| **403** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteOrgWebhook

> DeleteOrgWebhook200Response deleteOrgWebhook(orgId, webhookId)

Delete webhook

Permanently delete a webhook and all its delivery logs.

### Example

```ts
import {
  Configuration,
  WebhooksApi,
} from '@zippendo/sdk';
import type { DeleteOrgWebhookRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WebhooksApi(config);

  const body = {
    // string | Organization ID
    orgId: org_clx1a2b3c4,
    // string | Webhook ID
    webhookId: wh_clx1a2b3c4,
  } satisfies DeleteOrgWebhookRequest;

  try {
    const data = await api.deleteOrgWebhook(body);
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
| **webhookId** | `string` | Webhook ID | [Defaults to `undefined`] |

### Return type

[**DeleteOrgWebhook200Response**](DeleteOrgWebhook200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |
| **401** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getOrgWebhook

> CreateOrgWebhook201Response getOrgWebhook(orgId, webhookId)

Get webhook

Get a specific webhook including its signing secret.

### Example

```ts
import {
  Configuration,
  WebhooksApi,
} from '@zippendo/sdk';
import type { GetOrgWebhookRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WebhooksApi(config);

  const body = {
    // string | Organization ID
    orgId: org_clx1a2b3c4,
    // string | Webhook ID
    webhookId: wh_clx1a2b3c4,
  } satisfies GetOrgWebhookRequest;

  try {
    const data = await api.getOrgWebhook(body);
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
| **webhookId** | `string` | Webhook ID | [Defaults to `undefined`] |

### Return type

[**CreateOrgWebhook201Response**](CreateOrgWebhook201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |
| **401** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listOrgWebhookDeliveries

> ListOrgWebhookDeliveries200Response listOrgWebhookDeliveries(orgId, webhookId, page, limit)

List webhook deliveries

List the delivery history for a specific webhook.

### Example

```ts
import {
  Configuration,
  WebhooksApi,
} from '@zippendo/sdk';
import type { ListOrgWebhookDeliveriesRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WebhooksApi(config);

  const body = {
    // string | Organization ID
    orgId: org_clx1a2b3c4,
    // string | Webhook ID
    webhookId: wh_clx1a2b3c4,
    // number | Page number (1-based) (optional)
    page: 1,
    // number | Items per page (max 100) (optional)
    limit: 20,
  } satisfies ListOrgWebhookDeliveriesRequest;

  try {
    const data = await api.listOrgWebhookDeliveries(body);
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
| **webhookId** | `string` | Webhook ID | [Defaults to `undefined`] |
| **page** | `number` | Page number (1-based) | [Optional] [Defaults to `1`] |
| **limit** | `number` | Items per page (max 100) | [Optional] [Defaults to `20`] |

### Return type

[**ListOrgWebhookDeliveries200Response**](ListOrgWebhookDeliveries200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |
| **401** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listOrgWebhooks

> ListOrgWebhooks200Response listOrgWebhooks(orgId, page, limit)

List webhooks

List all webhooks belonging to an organization.

### Example

```ts
import {
  Configuration,
  WebhooksApi,
} from '@zippendo/sdk';
import type { ListOrgWebhooksRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WebhooksApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // number | Page number (1-based) (optional)
    page: 1,
    // number | Items per page (max 100) (optional)
    limit: 20,
  } satisfies ListOrgWebhooksRequest;

  try {
    const data = await api.listOrgWebhooks(body);
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

### Return type

[**ListOrgWebhooks200Response**](ListOrgWebhooks200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |
| **401** | Default Response |  -  |
| **403** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## testOrgWebhook

> TestOrgWebhook200Response testOrgWebhook(orgId, webhookId)

Test webhook

Send a test ping event to the webhook endpoint to verify connectivity.

### Example

```ts
import {
  Configuration,
  WebhooksApi,
} from '@zippendo/sdk';
import type { TestOrgWebhookRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WebhooksApi(config);

  const body = {
    // string | Organization ID
    orgId: org_clx1a2b3c4,
    // string | Webhook ID
    webhookId: wh_clx1a2b3c4,
  } satisfies TestOrgWebhookRequest;

  try {
    const data = await api.testOrgWebhook(body);
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
| **webhookId** | `string` | Webhook ID | [Defaults to `undefined`] |

### Return type

[**TestOrgWebhook200Response**](TestOrgWebhook200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |
| **401** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateOrgWebhook

> CreateOrgWebhook201Response updateOrgWebhook(orgId, webhookId, updateOrgWebhookRequest)

Update webhook

Update the configuration of an existing webhook.

### Example

```ts
import {
  Configuration,
  WebhooksApi,
} from '@zippendo/sdk';
import type { UpdateOrgWebhookOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WebhooksApi(config);

  const body = {
    // string | Organization ID
    orgId: org_clx1a2b3c4,
    // string | Webhook ID
    webhookId: wh_clx1a2b3c4,
    // UpdateOrgWebhookRequest
    updateOrgWebhookRequest: ...,
  } satisfies UpdateOrgWebhookOperationRequest;

  try {
    const data = await api.updateOrgWebhook(body);
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
| **webhookId** | `string` | Webhook ID | [Defaults to `undefined`] |
| **updateOrgWebhookRequest** | [UpdateOrgWebhookRequest](UpdateOrgWebhookRequest.md) |  | |

### Return type

[**CreateOrgWebhook201Response**](CreateOrgWebhook201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |
| **401** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

