# edgraph_platform_client.InstancesVendorsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_vendor_async**](InstancesVendorsApi.md#create_vendor_async) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/vendors | Creates a new Vendor.
[**delete_vendor_async**](InstancesVendorsApi.md#delete_vendor_async) | **DELETE** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/vendors/{vendorId} | Deletes a Vendor.
[**get_vendor_by_id_async**](InstancesVendorsApi.md#get_vendor_by_id_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/vendors/{vendorId} | Retrieves a Vendor by ID.
[**get_vendors_async**](InstancesVendorsApi.md#get_vendors_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/vendors | Retrieves a list of Vendors.
[**sync_vendor_async**](InstancesVendorsApi.md#sync_vendor_async) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/vendors/{vendorId}/sync | Copies a Vendor from one instance to another/other instance(s).
[**update_vendor_async**](InstancesVendorsApi.md#update_vendor_async) | **PUT** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/vendors/{vendorId} | Updates a Vendor.


# **create_vendor_async**
> EdfiAdminApiEdfiAdminV1VendorCreatedResponse create_vendor_async(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_create_vendor_request=edfi_admin_api_edfi_admin_v1_create_vendor_request)

Creates a new Vendor.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_vendor_request import EdfiAdminApiEdfiAdminV1CreateVendorRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_vendor_created_response import EdfiAdminApiEdfiAdminV1VendorCreatedResponse
from edgraph_platform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dev.edgraph.com/tenant
# See configuration.py for a list of all supported configuration parameters.
configuration = edgraph_platform_client.Configuration(
    host = "https://api.dev.edgraph.com/tenant"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.InstancesVendorsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_create_vendor_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1CreateVendorRequest() # EdfiAdminApiEdfiAdminV1CreateVendorRequest |  (optional)

    try:
        # Creates a new Vendor.
        api_response = await api_instance.create_vendor_async(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_create_vendor_request=edfi_admin_api_edfi_admin_v1_create_vendor_request)
        print("The response of InstancesVendorsApi->create_vendor_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesVendorsApi->create_vendor_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_create_vendor_request** | [**EdfiAdminApiEdfiAdminV1CreateVendorRequest**](EdfiAdminApiEdfiAdminV1CreateVendorRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1VendorCreatedResponse**](EdfiAdminApiEdfiAdminV1VendorCreatedResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**201** | The resource was created. The location of the resource is available in the Location header of the response. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_vendor_async**
> delete_vendor_async(tenant_id, instance_id, vendor_id)

Deletes a Vendor.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dev.edgraph.com/tenant
# See configuration.py for a list of all supported configuration parameters.
configuration = edgraph_platform_client.Configuration(
    host = "https://api.dev.edgraph.com/tenant"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.InstancesVendorsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    vendor_id = 56 # int | 

    try:
        # Deletes a Vendor.
        await api_instance.delete_vendor_async(tenant_id, instance_id, vendor_id)
    except Exception as e:
        print("Exception when calling InstancesVendorsApi->delete_vendor_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **vendor_id** | **int**|  | 

### Return type

void (empty response body)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**204** | The resource was successfully deleted. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_vendor_by_id_async**
> EdfiAdminApiEdfiAdminV1VendorProfileResponse get_vendor_by_id_async(tenant_id, instance_id, vendor_id)

Retrieves a Vendor by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_vendor_profile_response import EdfiAdminApiEdfiAdminV1VendorProfileResponse
from edgraph_platform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dev.edgraph.com/tenant
# See configuration.py for a list of all supported configuration parameters.
configuration = edgraph_platform_client.Configuration(
    host = "https://api.dev.edgraph.com/tenant"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.InstancesVendorsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    vendor_id = 'vendor_id_example' # str | 

    try:
        # Retrieves a Vendor by ID.
        api_response = await api_instance.get_vendor_by_id_async(tenant_id, instance_id, vendor_id)
        print("The response of InstancesVendorsApi->get_vendor_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesVendorsApi->get_vendor_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **vendor_id** | **str**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1VendorProfileResponse**](EdfiAdminApiEdfiAdminV1VendorProfileResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_vendors_async**
> EdfiAdminApiEdfiAdminV1VendorListResponsePaginatedItemsViewModel get_vendors_async(tenant_id, instance_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of Vendors.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_vendor_list_response_paginated_items_view_model import EdfiAdminApiEdfiAdminV1VendorListResponsePaginatedItemsViewModel
from edgraph_platform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dev.edgraph.com/tenant
# See configuration.py for a list of all supported configuration parameters.
configuration = edgraph_platform_client.Configuration(
    host = "https://api.dev.edgraph.com/tenant"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.InstancesVendorsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of Vendors.
        api_response = await api_instance.get_vendors_async(tenant_id, instance_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of InstancesVendorsApi->get_vendors_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesVendorsApi->get_vendors_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdfiAdminApiEdfiAdminV1VendorListResponsePaginatedItemsViewModel**](EdfiAdminApiEdfiAdminV1VendorListResponsePaginatedItemsViewModel.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **sync_vendor_async**
> sync_vendor_async(tenant_id, instance_id, vendor_id, edfi_admin_api_edfi_admin_v1_sync_vendor_request=edfi_admin_api_edfi_admin_v1_sync_vendor_request)

Copies a Vendor from one instance to another/other instance(s).

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_sync_vendor_request import EdfiAdminApiEdfiAdminV1SyncVendorRequest
from edgraph_platform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dev.edgraph.com/tenant
# See configuration.py for a list of all supported configuration parameters.
configuration = edgraph_platform_client.Configuration(
    host = "https://api.dev.edgraph.com/tenant"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.InstancesVendorsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    vendor_id = 56 # int | 
    edfi_admin_api_edfi_admin_v1_sync_vendor_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1SyncVendorRequest() # EdfiAdminApiEdfiAdminV1SyncVendorRequest |  (optional)

    try:
        # Copies a Vendor from one instance to another/other instance(s).
        await api_instance.sync_vendor_async(tenant_id, instance_id, vendor_id, edfi_admin_api_edfi_admin_v1_sync_vendor_request=edfi_admin_api_edfi_admin_v1_sync_vendor_request)
    except Exception as e:
        print("Exception when calling InstancesVendorsApi->sync_vendor_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **vendor_id** | **int**|  | 
 **edfi_admin_api_edfi_admin_v1_sync_vendor_request** | [**EdfiAdminApiEdfiAdminV1SyncVendorRequest**](EdfiAdminApiEdfiAdminV1SyncVendorRequest.md)|  | [optional] 

### Return type

void (empty response body)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_vendor_async**
> EdfiAdminApiEdfiAdminV1VendorUpdatedResponse update_vendor_async(tenant_id, instance_id, vendor_id, edfi_admin_api_edfi_admin_v1_update_vendor_request=edfi_admin_api_edfi_admin_v1_update_vendor_request)

Updates a Vendor.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_vendor_request import EdfiAdminApiEdfiAdminV1UpdateVendorRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_vendor_updated_response import EdfiAdminApiEdfiAdminV1VendorUpdatedResponse
from edgraph_platform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dev.edgraph.com/tenant
# See configuration.py for a list of all supported configuration parameters.
configuration = edgraph_platform_client.Configuration(
    host = "https://api.dev.edgraph.com/tenant"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.InstancesVendorsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    vendor_id = 'vendor_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_update_vendor_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1UpdateVendorRequest() # EdfiAdminApiEdfiAdminV1UpdateVendorRequest |  (optional)

    try:
        # Updates a Vendor.
        api_response = await api_instance.update_vendor_async(tenant_id, instance_id, vendor_id, edfi_admin_api_edfi_admin_v1_update_vendor_request=edfi_admin_api_edfi_admin_v1_update_vendor_request)
        print("The response of InstancesVendorsApi->update_vendor_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesVendorsApi->update_vendor_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **vendor_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_update_vendor_request** | [**EdfiAdminApiEdfiAdminV1UpdateVendorRequest**](EdfiAdminApiEdfiAdminV1UpdateVendorRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1VendorUpdatedResponse**](EdfiAdminApiEdfiAdminV1VendorUpdatedResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

