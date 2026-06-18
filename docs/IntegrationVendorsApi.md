# edgraph_platform_client.IntegrationVendorsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_integration_vendor**](IntegrationVendorsApi.md#create_integration_vendor) | **POST** /integrations/vendors | Creates an Integration Vendor.
[**delete_integration_vendor**](IntegrationVendorsApi.md#delete_integration_vendor) | **DELETE** /integrations/vendors/{vendorId} | Removes an Integration Vendor.
[**get_integration_vendor**](IntegrationVendorsApi.md#get_integration_vendor) | **GET** /integrations/vendors/{vendorId} | Gets an Integration Vendor.
[**search_integration_vendors**](IntegrationVendorsApi.md#search_integration_vendors) | **GET** /integrations/vendors | Search Integration Vendors.
[**update_integration_vendor**](IntegrationVendorsApi.md#update_integration_vendor) | **PUT** /integrations/vendors/{vendorId} | Updates an Integration Vendor.


# **create_integration_vendor**
> TenantApiIntegrationsV1CreateIntegrationVendorResponse create_integration_vendor(tenant_api_integrations_v1_create_integration_vendor_request=tenant_api_integrations_v1_create_integration_vendor_request)

Creates an Integration Vendor.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_create_integration_vendor_request import TenantApiIntegrationsV1CreateIntegrationVendorRequest
from edgraph_platform_client.models.tenant_api_integrations_v1_create_integration_vendor_response import TenantApiIntegrationsV1CreateIntegrationVendorResponse
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
    api_instance = edgraph_platform_client.IntegrationVendorsApi(api_client)
    tenant_api_integrations_v1_create_integration_vendor_request = edgraph_platform_client.TenantApiIntegrationsV1CreateIntegrationVendorRequest() # TenantApiIntegrationsV1CreateIntegrationVendorRequest |  (optional)

    try:
        # Creates an Integration Vendor.
        api_response = await api_instance.create_integration_vendor(tenant_api_integrations_v1_create_integration_vendor_request=tenant_api_integrations_v1_create_integration_vendor_request)
        print("The response of IntegrationVendorsApi->create_integration_vendor:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationVendorsApi->create_integration_vendor: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_api_integrations_v1_create_integration_vendor_request** | [**TenantApiIntegrationsV1CreateIntegrationVendorRequest**](TenantApiIntegrationsV1CreateIntegrationVendorRequest.md)|  | [optional] 

### Return type

[**TenantApiIntegrationsV1CreateIntegrationVendorResponse**](TenantApiIntegrationsV1CreateIntegrationVendorResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_integration_vendor**
> TenantApiIntegrationsV1DeleteIntegrationVendorResponse delete_integration_vendor(vendor_id)

Removes an Integration Vendor.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_delete_integration_vendor_response import TenantApiIntegrationsV1DeleteIntegrationVendorResponse
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
    api_instance = edgraph_platform_client.IntegrationVendorsApi(api_client)
    vendor_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Removes an Integration Vendor.
        api_response = await api_instance.delete_integration_vendor(vendor_id)
        print("The response of IntegrationVendorsApi->delete_integration_vendor:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationVendorsApi->delete_integration_vendor: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vendor_id** | **UUID**|  | 

### Return type

[**TenantApiIntegrationsV1DeleteIntegrationVendorResponse**](TenantApiIntegrationsV1DeleteIntegrationVendorResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_integration_vendor**
> TenantApiIntegrationsV1GetIntegrationVendorResponse get_integration_vendor(vendor_id)

Gets an Integration Vendor.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_get_integration_vendor_response import TenantApiIntegrationsV1GetIntegrationVendorResponse
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
    api_instance = edgraph_platform_client.IntegrationVendorsApi(api_client)
    vendor_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets an Integration Vendor.
        api_response = await api_instance.get_integration_vendor(vendor_id)
        print("The response of IntegrationVendorsApi->get_integration_vendor:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationVendorsApi->get_integration_vendor: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vendor_id** | **UUID**|  | 

### Return type

[**TenantApiIntegrationsV1GetIntegrationVendorResponse**](TenantApiIntegrationsV1GetIntegrationVendorResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **search_integration_vendors**
> TenantApiIntegrationsV1IntegrationVendorPaginatedItemsViewModel search_integration_vendors(page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Search Integration Vendors.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_integration_vendor_paginated_items_view_model import TenantApiIntegrationsV1IntegrationVendorPaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.IntegrationVendorsApi(api_client)
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Search Integration Vendors.
        api_response = await api_instance.search_integration_vendors(page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of IntegrationVendorsApi->search_integration_vendors:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationVendorsApi->search_integration_vendors: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**TenantApiIntegrationsV1IntegrationVendorPaginatedItemsViewModel**](TenantApiIntegrationsV1IntegrationVendorPaginatedItemsViewModel.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_integration_vendor**
> object update_integration_vendor(vendor_id, tenant_api_integrations_v1_update_integration_vendor_request=tenant_api_integrations_v1_update_integration_vendor_request)

Updates an Integration Vendor.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_update_integration_vendor_request import TenantApiIntegrationsV1UpdateIntegrationVendorRequest
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
    api_instance = edgraph_platform_client.IntegrationVendorsApi(api_client)
    vendor_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    tenant_api_integrations_v1_update_integration_vendor_request = edgraph_platform_client.TenantApiIntegrationsV1UpdateIntegrationVendorRequest() # TenantApiIntegrationsV1UpdateIntegrationVendorRequest |  (optional)

    try:
        # Updates an Integration Vendor.
        api_response = await api_instance.update_integration_vendor(vendor_id, tenant_api_integrations_v1_update_integration_vendor_request=tenant_api_integrations_v1_update_integration_vendor_request)
        print("The response of IntegrationVendorsApi->update_integration_vendor:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationVendorsApi->update_integration_vendor: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vendor_id** | **UUID**|  | 
 **tenant_api_integrations_v1_update_integration_vendor_request** | [**TenantApiIntegrationsV1UpdateIntegrationVendorRequest**](TenantApiIntegrationsV1UpdateIntegrationVendorRequest.md)|  | [optional] 

### Return type

**object**

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

