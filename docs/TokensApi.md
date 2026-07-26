# TokensApi

All URIs are relative to *https://api.zippendo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createApiToken**](TokensApi.md#createapitokenoperation) | **POST** /orgs/{orgId}/api-tokens | Create API keys |
| [**getApiToken**](TokensApi.md#getapitoken) | **GET** /orgs/{orgId}/api-tokens/{tokenId} | Get API keys |
| [**listApiTokens**](TokensApi.md#listapitokens) | **GET** /orgs/{orgId}/api-tokens | List API keys |
| [**revokeApiToken**](TokensApi.md#revokeapitoken) | **DELETE** /orgs/{orgId}/api-tokens/{tokenId} | Revoke API keys |
| [**updateApiToken**](TokensApi.md#updateapitokenoperation) | **PATCH** /orgs/{orgId}/api-tokens/{tokenId} | Update API keys |
| [**verifyApiToken**](TokensApi.md#verifyapitokenoperation) | **POST** /api-tokens/verify | Verify API keys |



## createApiToken

> CreateApiToken201Response createApiToken(orgId, createApiTokenRequest)

Create API keys

Creates a new API token for the specified organization. The full token is only shown once.

### Example

```ts
import {
  Configuration,
  TokensApi,
} from '@zippendo/sdk';
import type { CreateApiTokenOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TokensApi(config);

  const body = {
    // string | Organization ID
    orgId: org_4d8af01qw2,
    // CreateApiTokenRequest
    createApiTokenRequest: ...,
  } satisfies CreateApiTokenOperationRequest;

  try {
    const data = await api.createApiToken(body);
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
| **createApiTokenRequest** | [CreateApiTokenRequest](CreateApiTokenRequest.md) |  | |

### Return type

[**CreateApiToken201Response**](CreateApiToken201Response.md)

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


## getApiToken

> ListApiTokens200ResponseDataInner getApiToken(orgId, tokenId)

Get API keys

Returns metadata for a specific API token. The token secret is never returned.

### Example

```ts
import {
  Configuration,
  TokensApi,
} from '@zippendo/sdk';
import type { GetApiTokenRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TokensApi(config);

  const body = {
    // string | Organization ID
    orgId: org_4d8af01qw2,
    // string | API Token ID
    tokenId: tok_6e2fa83ij9,
  } satisfies GetApiTokenRequest;

  try {
    const data = await api.getApiToken(body);
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
| **tokenId** | `string` | API Token ID | [Defaults to `undefined`] |

### Return type

[**ListApiTokens200ResponseDataInner**](ListApiTokens200ResponseDataInner.md)

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


## listApiTokens

> ListApiTokens200Response listApiTokens(orgId, page, limit)

List API keys

Returns a paginated list of API tokens belonging to the specified organization.

### Example

```ts
import {
  Configuration,
  TokensApi,
} from '@zippendo/sdk';
import type { ListApiTokensRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TokensApi(config);

  const body = {
    // string | Organization ID
    orgId: org_4d8af01qw2,
    // number | Page number (1-based) (optional)
    page: 1,
    // number | Items per page (max 100) (optional)
    limit: 20,
  } satisfies ListApiTokensRequest;

  try {
    const data = await api.listApiTokens(body);
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

[**ListApiTokens200Response**](ListApiTokens200Response.md)

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


## revokeApiToken

> RevokeApiToken200Response revokeApiToken(orgId, tokenId)

Revoke API keys

Revokes and deletes an API token.

### Example

```ts
import {
  Configuration,
  TokensApi,
} from '@zippendo/sdk';
import type { RevokeApiTokenRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TokensApi(config);

  const body = {
    // string | Organization ID
    orgId: org_4d8af01qw2,
    // string | API Token ID
    tokenId: tok_6e2fa83ij9,
  } satisfies RevokeApiTokenRequest;

  try {
    const data = await api.revokeApiToken(body);
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
| **tokenId** | `string` | API Token ID | [Defaults to `undefined`] |

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
| **401** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateApiToken

> ListApiTokens200ResponseDataInner updateApiToken(orgId, tokenId, updateApiTokenRequest)

Update API keys

Updates the name of an API token.

### Example

```ts
import {
  Configuration,
  TokensApi,
} from '@zippendo/sdk';
import type { UpdateApiTokenOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TokensApi(config);

  const body = {
    // string | Organization ID
    orgId: org_4d8af01qw2,
    // string | API Token ID
    tokenId: tok_6e2fa83ij9,
    // UpdateApiTokenRequest
    updateApiTokenRequest: ...,
  } satisfies UpdateApiTokenOperationRequest;

  try {
    const data = await api.updateApiToken(body);
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
| **tokenId** | `string` | API Token ID | [Defaults to `undefined`] |
| **updateApiTokenRequest** | [UpdateApiTokenRequest](UpdateApiTokenRequest.md) |  | |

### Return type

[**ListApiTokens200ResponseDataInner**](ListApiTokens200ResponseDataInner.md)

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


## verifyApiToken

> VerifyApiToken200Response verifyApiToken(verifyApiTokenRequest)

Verify API keys

Verifies whether an API token is valid and returns its metadata.

### Example

```ts
import {
  Configuration,
  TokensApi,
} from '@zippendo/sdk';
import type { VerifyApiTokenOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TokensApi(config);

  const body = {
    // VerifyApiTokenRequest
    verifyApiTokenRequest: ...,
  } satisfies VerifyApiTokenOperationRequest;

  try {
    const data = await api.verifyApiToken(body);
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
| **verifyApiTokenRequest** | [VerifyApiTokenRequest](VerifyApiTokenRequest.md) |  | |

### Return type

[**VerifyApiToken200Response**](VerifyApiToken200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

