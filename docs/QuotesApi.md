# QuotesApi

All URIs are relative to *https://api.zippendo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createShippingQuote**](QuotesApi.md#createshippingquoteoperation) | **POST** /orgs/{orgId}/shipping-quote | Calculate shipping rates |



## createShippingQuote

> CreateShippingQuote200Response createShippingQuote(orgId, createShippingQuoteRequest)

Calculate shipping rates

Calculates shipping rates from configured shipping rules based on cart items and destination.

### Example

```ts
import {
  Configuration,
  QuotesApi,
} from '@zippendo/sdk';
import type { CreateShippingQuoteOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new QuotesApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
    // CreateShippingQuoteRequest
    createShippingQuoteRequest: ...,
  } satisfies CreateShippingQuoteOperationRequest;

  try {
    const data = await api.createShippingQuote(body);
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
| **createShippingQuoteRequest** | [CreateShippingQuoteRequest](CreateShippingQuoteRequest.md) |  | |

### Return type

[**CreateShippingQuote200Response**](CreateShippingQuote200Response.md)

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
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

