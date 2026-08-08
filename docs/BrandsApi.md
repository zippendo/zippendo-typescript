# BrandsApi

All URIs are relative to *https://api.zippendo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**archiveOrgBrand**](BrandsApi.md#archiveorgbrand) | **POST** /orgs/{orgId}/brands/{brandId}/archive | Archive brand |
| [**checkBrandSlug**](BrandsApi.md#checkbrandslug) | **GET** /orgs/{orgId}/brands/check-slug/{slug} | Check brand slug availability |
| [**createOrgBrand**](BrandsApi.md#createorgbrandoperation) | **POST** /orgs/{orgId}/brands | Create brand |
| [**deleteBrandLogo**](BrandsApi.md#deletebrandlogo) | **DELETE** /orgs/{orgId}/brands/{brandId}/logo | Delete brand logo |
| [**getBrandLogo**](BrandsApi.md#getbrandlogo) | **GET** /orgs/{orgId}/brands/{brandId}/logo | Get brand logo |
| [**getOrgBrand**](BrandsApi.md#getorgbrand) | **GET** /orgs/{orgId}/brands/{brandId} | Get brand |
| [**listOrgBrands**](BrandsApi.md#listorgbrands) | **GET** /orgs/{orgId}/brands | List brands |
| [**unarchiveOrgBrand**](BrandsApi.md#unarchiveorgbrand) | **POST** /orgs/{orgId}/brands/{brandId}/unarchive | Unarchive brand |
| [**updateOrgBrand**](BrandsApi.md#updateorgbrandoperation) | **PATCH** /orgs/{orgId}/brands/{brandId} | Update brand |
| [**uploadBrandLogo**](BrandsApi.md#uploadbrandlogo) | **POST** /orgs/{orgId}/brands/{brandId}/logo | Upload brand logo |



## archiveOrgBrand

> ListOrgBrands200ResponseDataInner archiveOrgBrand(orgId, brandId)

Archive brand

Archives a brand: it leaves the brand switcher and default listings, but its orders, shipments and settings are retained and remain visible in the organization-wide view.

### Example

```ts
import {
  Configuration,
  BrandsApi,
} from '@zippendo/sdk';
import type { ArchiveOrgBrandRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BrandsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // string | Brand ID
    brandId: brnd_8f3kd92ld0,
  } satisfies ArchiveOrgBrandRequest;

  try {
    const data = await api.archiveOrgBrand(body);
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
| **brandId** | `string` | Brand ID | [Defaults to `undefined`] |

### Return type

[**ListOrgBrands200ResponseDataInner**](ListOrgBrands200ResponseDataInner.md)

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


## checkBrandSlug

> CheckBrandSlug200Response checkBrandSlug(orgId, slug)

Check brand slug availability

Reports whether a brand slug is free within this organization. Brand slugs are unique per organization, so the same slug may exist in another organization. Archived brands still hold their slug.

### Example

```ts
import {
  Configuration,
  BrandsApi,
} from '@zippendo/sdk';
import type { CheckBrandSlugRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BrandsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // string | Brand slug to check
    slug: acme,
  } satisfies CheckBrandSlugRequest;

  try {
    const data = await api.checkBrandSlug(body);
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
| **slug** | `string` | Brand slug to check | [Defaults to `undefined`] |

### Return type

[**CheckBrandSlug200Response**](CheckBrandSlug200Response.md)

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
| **401** | Default Response |  -  |
| **403** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createOrgBrand

> ListOrgBrands200ResponseDataInner createOrgBrand(orgId, createOrgBrandRequest)

Create brand

Creates a brand (sub-account) in the organization. The slug is derived from the name when omitted. Requires a plan that includes brands.

### Example

```ts
import {
  Configuration,
  BrandsApi,
} from '@zippendo/sdk';
import type { CreateOrgBrandOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BrandsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // CreateOrgBrandRequest
    createOrgBrandRequest: ...,
  } satisfies CreateOrgBrandOperationRequest;

  try {
    const data = await api.createOrgBrand(body);
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
| **createOrgBrandRequest** | [CreateOrgBrandRequest](CreateOrgBrandRequest.md) |  | |

### Return type

[**ListOrgBrands200ResponseDataInner**](ListOrgBrands200ResponseDataInner.md)

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
| **409** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteBrandLogo

> ListOrgBrands200ResponseDataInner deleteBrandLogo(orgId, brandId)

Delete brand logo

Removes a brand\&#39;s logo. Its documents fall back to the organization\&#39;s logo. Requires the brands and customBranding entitlements.

### Example

```ts
import {
  Configuration,
  BrandsApi,
} from '@zippendo/sdk';
import type { DeleteBrandLogoRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BrandsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // string | Brand ID
    brandId: brnd_8f3kd92ld0,
  } satisfies DeleteBrandLogoRequest;

  try {
    const data = await api.deleteBrandLogo(body);
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
| **brandId** | `string` | Brand ID | [Defaults to `undefined`] |

### Return type

[**ListOrgBrands200ResponseDataInner**](ListOrgBrands200ResponseDataInner.md)

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


## getBrandLogo

> Blob getBrandLogo(orgId, brandId)

Get brand logo

Streams the brand\&#39;s logo bytes. This is the URL returned as the brand\&#39;s &#x60;logoUrl&#x60;.

### Example

```ts
import {
  Configuration,
  BrandsApi,
} from '@zippendo/sdk';
import type { GetBrandLogoRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BrandsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // string | Brand ID
    brandId: brnd_8f3kd92ld0,
  } satisfies GetBrandLogoRequest;

  try {
    const data = await api.getBrandLogo(body);
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
| **brandId** | `string` | Brand ID | [Defaults to `undefined`] |

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
| **401** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getOrgBrand

> ListOrgBrands200ResponseDataInner getOrgBrand(orgId, brandId)

Get brand

Returns a single brand (sub-account) by id.

### Example

```ts
import {
  Configuration,
  BrandsApi,
} from '@zippendo/sdk';
import type { GetOrgBrandRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BrandsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // string | Brand ID
    brandId: brnd_8f3kd92ld0,
  } satisfies GetOrgBrandRequest;

  try {
    const data = await api.getOrgBrand(body);
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
| **brandId** | `string` | Brand ID | [Defaults to `undefined`] |

### Return type

[**ListOrgBrands200ResponseDataInner**](ListOrgBrands200ResponseDataInner.md)

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


## listOrgBrands

> ListOrgBrands200Response listOrgBrands(orgId, includeArchived)

List brands

Returns the organization\&#39;s brands (sub-accounts). Archived brands are excluded unless &#x60;includeArchived&#x60; is set.

### Example

```ts
import {
  Configuration,
  BrandsApi,
} from '@zippendo/sdk';
import type { ListOrgBrandsRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BrandsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // string | Include archived brands in the response (optional)
    includeArchived: false,
  } satisfies ListOrgBrandsRequest;

  try {
    const data = await api.listOrgBrands(body);
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
| **includeArchived** | `string` | Include archived brands in the response | [Optional] [Defaults to `undefined`] |

### Return type

[**ListOrgBrands200Response**](ListOrgBrands200Response.md)

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


## unarchiveOrgBrand

> ListOrgBrands200ResponseDataInner unarchiveOrgBrand(orgId, brandId)

Unarchive brand

Restores an archived brand so it appears in the brand switcher again.

### Example

```ts
import {
  Configuration,
  BrandsApi,
} from '@zippendo/sdk';
import type { UnarchiveOrgBrandRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BrandsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // string | Brand ID
    brandId: brnd_8f3kd92ld0,
  } satisfies UnarchiveOrgBrandRequest;

  try {
    const data = await api.unarchiveOrgBrand(body);
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
| **brandId** | `string` | Brand ID | [Defaults to `undefined`] |

### Return type

[**ListOrgBrands200ResponseDataInner**](ListOrgBrands200ResponseDataInner.md)

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


## updateOrgBrand

> ListOrgBrands200ResponseDataInner updateOrgBrand(orgId, brandId, updateOrgBrandRequest)

Update brand

Updates a brand\&#39;s name, slug, identity overrides (company name, VAT, customs, address) and document colours. Null clears an override so the organization\&#39;s value applies again.

### Example

```ts
import {
  Configuration,
  BrandsApi,
} from '@zippendo/sdk';
import type { UpdateOrgBrandOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BrandsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // string | Brand ID
    brandId: brnd_8f3kd92ld0,
    // UpdateOrgBrandRequest
    updateOrgBrandRequest: ...,
  } satisfies UpdateOrgBrandOperationRequest;

  try {
    const data = await api.updateOrgBrand(body);
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
| **brandId** | `string` | Brand ID | [Defaults to `undefined`] |
| **updateOrgBrandRequest** | [UpdateOrgBrandRequest](UpdateOrgBrandRequest.md) |  | |

### Return type

[**ListOrgBrands200ResponseDataInner**](ListOrgBrands200ResponseDataInner.md)

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
| **409** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## uploadBrandLogo

> ListOrgBrands200ResponseDataInner uploadBrandLogo(orgId, brandId, file)

Upload brand logo

Uploads a brand\&#39;s logo as multipart/form-data. Accepts PNG, JPG or WEBP up to 5MB and 4096×4096px; the image is re-encoded and stored. Documents for this brand\&#39;s shipments use it instead of the organization\&#39;s logo. Requires the brands and customBranding entitlements.

### Example

```ts
import {
  Configuration,
  BrandsApi,
} from '@zippendo/sdk';
import type { UploadBrandLogoRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BrandsApi(config);

  const body = {
    // string | Organization ID
    orgId: org_8f3kd92ld0,
    // string | Brand ID
    brandId: brnd_8f3kd92ld0,
    // Blob | Image file (PNG, JPG, or WEBP)
    file: BINARY_DATA_HERE,
  } satisfies UploadBrandLogoRequest;

  try {
    const data = await api.uploadBrandLogo(body);
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
| **brandId** | `string` | Brand ID | [Defaults to `undefined`] |
| **file** | `Blob` | Image file (PNG, JPG, or WEBP) | [Defaults to `undefined`] |

### Return type

[**ListOrgBrands200ResponseDataInner**](ListOrgBrands200ResponseDataInner.md)

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

