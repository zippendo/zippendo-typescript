# CarrierCatalogApi

All URIs are relative to *https://api.zippendo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**listAvailableCarriers**](CarrierCatalogApi.md#listavailablecarriers) | **GET** /orgs/{orgId}/available-carriers | List available carriers |



## listAvailableCarriers

> Array&lt;ListAvailableCarriers200ResponseInner&gt; listAvailableCarriers(orgId)

List available carriers

Returns the carriers available to connect, as supported by the carrier server.

### Example

```ts
import {
  Configuration,
  CarrierCatalogApi,
} from '@zippendo/sdk';
import type { ListAvailableCarriersRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CarrierCatalogApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
  } satisfies ListAvailableCarriersRequest;

  try {
    const data = await api.listAvailableCarriers(body);
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

[**Array&lt;ListAvailableCarriers200ResponseInner&gt;**](ListAvailableCarriers200ResponseInner.md)

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
| **500** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

