# BillingApi

All URIs are relative to *https://api.zippendo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getBillingUsage**](BillingApi.md#getbillingusage) | **GET** /orgs/{orgId}/billing/usage | Get usage |



## getBillingUsage

> GetBillingUsage200Response getBillingUsage(orgId)

Get usage

Get detailed usage statistics for the current billing period.

### Example

```ts
import {
  Configuration,
  BillingApi,
} from '@zippendo/sdk';
import type { GetBillingUsageRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BillingApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
  } satisfies GetBillingUsageRequest;

  try {
    const data = await api.getBillingUsage(body);
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

### Return type

[**GetBillingUsage200Response**](GetBillingUsage200Response.md)

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

