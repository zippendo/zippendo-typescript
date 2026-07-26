# AddressesApi

All URIs are relative to *https://api.zippendo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createAddress**](AddressesApi.md#createaddressoperation) | **POST** /orgs/{orgId}/addresses | Create address |
| [**deleteAddress**](AddressesApi.md#deleteaddress) | **DELETE** /orgs/{orgId}/addresses/{addressId} | Delete address |
| [**getAddress**](AddressesApi.md#getaddress) | **GET** /orgs/{orgId}/addresses/{addressId} | Get address |
| [**listAddresses**](AddressesApi.md#listaddresses) | **GET** /orgs/{orgId}/addresses | List addresses |
| [**updateAddress**](AddressesApi.md#updateaddressoperation) | **PUT** /orgs/{orgId}/addresses/{addressId} | Update address |



## createAddress

> ListAddresses200ResponseDataInner createAddress(orgId, createAddressRequest)

Create address

Creates a new sender, pickup or return address for the organization.

### Example

```ts
import {
  Configuration,
  AddressesApi,
} from '@zippendo/sdk';
import type { CreateAddressOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AddressesApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
    // CreateAddressRequest
    createAddressRequest: ...,
  } satisfies CreateAddressOperationRequest;

  try {
    const data = await api.createAddress(body);
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
| **createAddressRequest** | [CreateAddressRequest](CreateAddressRequest.md) |  | |

### Return type

[**ListAddresses200ResponseDataInner**](ListAddresses200ResponseDataInner.md)

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


## deleteAddress

> string deleteAddress(orgId, addressId)

Delete address

Deletes an address belonging to the organization.

### Example

```ts
import {
  Configuration,
  AddressesApi,
} from '@zippendo/sdk';
import type { DeleteAddressRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AddressesApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
    // string | Address ID
    addressId: addr_01HZX9K2QF,
  } satisfies DeleteAddressRequest;

  try {
    const data = await api.deleteAddress(body);
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
| **addressId** | `string` | Address ID | [Defaults to `undefined`] |

### Return type

**string**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Default Response |  -  |
| **403** | Default Response |  -  |
| **404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getAddress

> ListAddresses200ResponseDataInner getAddress(orgId, addressId)

Get address

Returns a single address belonging to the organization, identified by its ID.

### Example

```ts
import {
  Configuration,
  AddressesApi,
} from '@zippendo/sdk';
import type { GetAddressRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AddressesApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
    // string | Address ID
    addressId: addr_01HZX9K2QF,
  } satisfies GetAddressRequest;

  try {
    const data = await api.getAddress(body);
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
| **addressId** | `string` | Address ID | [Defaults to `undefined`] |

### Return type

[**ListAddresses200ResponseDataInner**](ListAddresses200ResponseDataInner.md)

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


## listAddresses

> ListAddresses200Response listAddresses(orgId, page, limit, type)

List addresses

Returns a paginated list of addresses for the organization, optionally filtered by type.

### Example

```ts
import {
  Configuration,
  AddressesApi,
} from '@zippendo/sdk';
import type { ListAddressesRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AddressesApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
    // number | Page number (1-based) (optional)
    page: 1,
    // number | Items per page (max 100) (optional)
    limit: 20,
    // 'sender' | 'pickup' | 'return' | Filter by address type (sender, pickup, return) (optional)
    type: sender,
  } satisfies ListAddressesRequest;

  try {
    const data = await api.listAddresses(body);
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
| **type** | `sender`, `pickup`, `return` | Filter by address type (sender, pickup, return) | [Optional] [Defaults to `undefined`] [Enum: sender, pickup, return] |

### Return type

[**ListAddresses200Response**](ListAddresses200Response.md)

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


## updateAddress

> ListAddresses200ResponseDataInner updateAddress(orgId, addressId, updateAddressRequest)

Update address

Updates an existing address belonging to the organization.

### Example

```ts
import {
  Configuration,
  AddressesApi,
} from '@zippendo/sdk';
import type { UpdateAddressOperationRequest } from '@zippendo/sdk';

async function example() {
  console.log("🚀 Testing @zippendo/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AddressesApi(config);

  const body = {
    // string | Organization ID
    orgId: org_01HZX9K2QF,
    // string | Address ID
    addressId: addr_01HZX9K2QF,
    // UpdateAddressRequest
    updateAddressRequest: ...,
  } satisfies UpdateAddressOperationRequest;

  try {
    const data = await api.updateAddress(body);
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
| **addressId** | `string` | Address ID | [Defaults to `undefined`] |
| **updateAddressRequest** | [UpdateAddressRequest](UpdateAddressRequest.md) |  | |

### Return type

[**ListAddresses200ResponseDataInner**](ListAddresses200ResponseDataInner.md)

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

