# RulesApi

All URIs are relative to *https://api.zippendo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createShippingRule**](RulesApi.md#createshippingruleoperation) | **POST** /orgs/{orgId}/shipping-rules | Create shipping rule |
| [**deleteShippingRule**](RulesApi.md#deleteshippingrule) | **DELETE** /orgs/{orgId}/shipping-rules/{ruleId} | Delete shipping rule |
| [**getShippingRule**](RulesApi.md#getshippingrule) | **GET** /orgs/{orgId}/shipping-rules/{ruleId} | Get shipping rule |
| [**listShippingRules**](RulesApi.md#listshippingrules) | **GET** /orgs/{orgId}/shipping-rules | List shipping rules |
| [**updateShippingRule**](RulesApi.md#updateshippingruleoperation) | **PATCH** /orgs/{orgId}/shipping-rules/{ruleId} | Update shipping rule |



## createShippingRule

> CreateShippingRule201Response createShippingRule(orgId, createShippingRuleRequest)

Create shipping rule

Creates a new shipping rule with conditions and carrier product for the organization.

### Example

```ts
import {
  Configuration,
  RulesApi,
} from '@zippendo/sdk';
import type { CreateShippingRuleOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RulesApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
    // CreateShippingRuleRequest
    createShippingRuleRequest: ...,
  } satisfies CreateShippingRuleOperationRequest;

  try {
    const data = await api.createShippingRule(body);
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
| **createShippingRuleRequest** | [CreateShippingRuleRequest](CreateShippingRuleRequest.md) |  | |

### Return type

[**CreateShippingRule201Response**](CreateShippingRule201Response.md)

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


## deleteShippingRule

> DeleteShippingRule200Response deleteShippingRule(orgId, ruleId)

Delete shipping rule

Deletes a shipping rule belonging to the organization.

### Example

```ts
import {
  Configuration,
  RulesApi,
} from '@zippendo/sdk';
import type { DeleteShippingRuleRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RulesApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
    // string | Shipping Rule ID
    ruleId: rule_01HZX9K2QF,
  } satisfies DeleteShippingRuleRequest;

  try {
    const data = await api.deleteShippingRule(body);
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
| **ruleId** | `string` | Shipping Rule ID | [Defaults to `undefined`] |

### Return type

[**DeleteShippingRule200Response**](DeleteShippingRule200Response.md)

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


## getShippingRule

> ListShippingRules200ResponseDataInner getShippingRule(orgId, ruleId)

Get shipping rule

Returns a single shipping rule with its carrier, address and printer relations.

### Example

```ts
import {
  Configuration,
  RulesApi,
} from '@zippendo/sdk';
import type { GetShippingRuleRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RulesApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
    // string | Shipping Rule ID
    ruleId: rule_01HZX9K2QF,
  } satisfies GetShippingRuleRequest;

  try {
    const data = await api.getShippingRule(body);
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
| **ruleId** | `string` | Shipping Rule ID | [Defaults to `undefined`] |

### Return type

[**ListShippingRules200ResponseDataInner**](ListShippingRules200ResponseDataInner.md)

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


## listShippingRules

> ListShippingRules200Response listShippingRules(orgId, page, limit)

List shipping rules

Returns a paginated list of shipping rules for the organization with their relations.

### Example

```ts
import {
  Configuration,
  RulesApi,
} from '@zippendo/sdk';
import type { ListShippingRulesRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RulesApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
    // number | Page number (1-based) (optional)
    page: 1,
    // number | Items per page (max 100) (optional)
    limit: 20,
  } satisfies ListShippingRulesRequest;

  try {
    const data = await api.listShippingRules(body);
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

[**ListShippingRules200Response**](ListShippingRules200Response.md)

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


## updateShippingRule

> CreateShippingRule201Response updateShippingRule(orgId, ruleId, updateShippingRuleRequest)

Update shipping rule

Updates an existing shipping rule for the organization.

### Example

```ts
import {
  Configuration,
  RulesApi,
} from '@zippendo/sdk';
import type { UpdateShippingRuleOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RulesApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
    // string | Shipping Rule ID
    ruleId: rule_01HZX9K2QF,
    // UpdateShippingRuleRequest
    updateShippingRuleRequest: ...,
  } satisfies UpdateShippingRuleOperationRequest;

  try {
    const data = await api.updateShippingRule(body);
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
| **ruleId** | `string` | Shipping Rule ID | [Defaults to `undefined`] |
| **updateShippingRuleRequest** | [UpdateShippingRuleRequest](UpdateShippingRuleRequest.md) |  | |

### Return type

[**CreateShippingRule201Response**](CreateShippingRule201Response.md)

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

