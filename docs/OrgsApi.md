# OrgsApi

All URIs are relative to *https://api.zippendo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**deleteOrgLogo**](OrgsApi.md#deleteorglogo) | **DELETE** /orgs/{orgId}/branding/logo | Delete org logo |
| [**getOrg**](OrgsApi.md#getorg) | **GET** /orgs/{id} | Get org |
| [**getOrgBranding**](OrgsApi.md#getorgbranding) | **GET** /orgs/{orgId}/branding | Get org branding |
| [**getOrgLogo**](OrgsApi.md#getorglogo) | **GET** /orgs/{orgId}/branding/logo | Download org logo |
| [**updateOrg**](OrgsApi.md#updateorgoperation) | **PUT** /orgs/{id} | Update org |
| [**updateOrgBranding**](OrgsApi.md#updateorgbrandingoperation) | **PUT** /orgs/{orgId}/branding | Update org branding |
| [**uploadOrgLogo**](OrgsApi.md#uploadorglogo) | **POST** /orgs/{orgId}/branding/logo | Upload org logo |



## deleteOrgLogo

> GetOrgBranding200Response deleteOrgLogo(orgId)

Delete org logo

Removes the org logo. Requires the customBranding entitlement.

### Example

```ts
import {
  Configuration,
  OrgsApi,
} from '@zippendo/sdk';
import type { DeleteOrgLogoRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrgsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
  } satisfies DeleteOrgLogoRequest;

  try {
    const data = await api.deleteOrgLogo(body);
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

[**GetOrgBranding200Response**](GetOrgBranding200Response.md)

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


## getOrg

> GetOrg200Response getOrg(id)

Get org

Returns a specific organization by ID, including its member count.

### Example

```ts
import {
  Configuration,
  OrgsApi,
} from '@zippendo/sdk';
import type { GetOrgRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrgsApi(config);

  const body = {
    // string | Resource ID
    id: clz9x8a7b0001,
  } satisfies GetOrgRequest;

  try {
    const data = await api.getOrg(body);
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
| **id** | `string` | Resource ID | [Defaults to `undefined`] |

### Return type

[**GetOrg200Response**](GetOrg200Response.md)

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


## getOrgBranding

> GetOrgBranding200Response getOrgBranding(orgId)

Get org branding

Returns the org\&#39;s brand colors and an authenticated URL to download the logo.

### Example

```ts
import {
  Configuration,
  OrgsApi,
} from '@zippendo/sdk';
import type { GetOrgBrandingRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrgsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
  } satisfies GetOrgBrandingRequest;

  try {
    const data = await api.getOrgBranding(body);
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

[**GetOrgBranding200Response**](GetOrgBranding200Response.md)

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


## getOrgLogo

> Blob getOrgLogo(orgId)

Download org logo

Returns the org logo image bytes with the stored content type.

### Example

```ts
import {
  Configuration,
  OrgsApi,
} from '@zippendo/sdk';
import type { GetOrgLogoRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrgsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
  } satisfies GetOrgLogoRequest;

  try {
    const data = await api.getOrgLogo(body);
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

**Blob**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `image/png`, `image/jpeg`, `image/webp`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | The logo image bytes |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateOrg

> UpdateOrg200Response updateOrg(id, updateOrgRequest)

Update org

Updates an existing organization\&#39;s profile, billing, and customs settings.

### Example

```ts
import {
  Configuration,
  OrgsApi,
} from '@zippendo/sdk';
import type { UpdateOrgOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrgsApi(config);

  const body = {
    // string | Resource ID
    id: clz9x8a7b0001,
    // UpdateOrgRequest
    updateOrgRequest: ...,
  } satisfies UpdateOrgOperationRequest;

  try {
    const data = await api.updateOrg(body);
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
| **id** | `string` | Resource ID | [Defaults to `undefined`] |
| **updateOrgRequest** | [UpdateOrgRequest](UpdateOrgRequest.md) |  | |

### Return type

[**UpdateOrg200Response**](UpdateOrg200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateOrgBranding

> GetOrgBranding200Response updateOrgBranding(orgId, updateOrgBrandingRequest)

Update org branding

Sets the org brand colors. Requires the customBranding entitlement.

### Example

```ts
import {
  Configuration,
  OrgsApi,
} from '@zippendo/sdk';
import type { UpdateOrgBrandingOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrgsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // UpdateOrgBrandingRequest
    updateOrgBrandingRequest: ...,
  } satisfies UpdateOrgBrandingOperationRequest;

  try {
    const data = await api.updateOrgBranding(body);
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
| **updateOrgBrandingRequest** | [UpdateOrgBrandingRequest](UpdateOrgBrandingRequest.md) |  | |

### Return type

[**GetOrgBranding200Response**](GetOrgBranding200Response.md)

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


## uploadOrgLogo

> GetOrgBranding200Response uploadOrgLogo(orgId, file)

Upload org logo

Uploads the org logo as multipart/form-data. Accepts PNG, JPG, or WEBP up to 5MB and 4096×4096px; the image is re-encoded and stored. Requires the customBranding entitlement.

### Example

```ts
import {
  Configuration,
  OrgsApi,
} from '@zippendo/sdk';
import type { UploadOrgLogoRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrgsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // Blob | Image file (PNG, JPG, or WEBP)
    file: BINARY_DATA_HERE,
  } satisfies UploadOrgLogoRequest;

  try {
    const data = await api.uploadOrgLogo(body);
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
| **file** | `Blob` | Image file (PNG, JPG, or WEBP) | [Defaults to `undefined`] |

### Return type

[**GetOrgBranding200Response**](GetOrgBranding200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default Response |  -  |
| **400** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |
| **413** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

