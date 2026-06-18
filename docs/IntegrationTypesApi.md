# edgraph_platform_client.IntegrationTypesApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_integration_type**](IntegrationTypesApi.md#create_integration_type) | **POST** /integrations/types | Creates an Integration Type.
[**delete_integration_type**](IntegrationTypesApi.md#delete_integration_type) | **DELETE** /integrations/types/{typeId} | Removes an Integration Type.
[**get_integration_type**](IntegrationTypesApi.md#get_integration_type) | **GET** /integrations/types/{typeId} | Gets an Integration Type.
[**search_integration_types**](IntegrationTypesApi.md#search_integration_types) | **GET** /integrations/types | Search Integration Types.
[**update_integration_type**](IntegrationTypesApi.md#update_integration_type) | **PUT** /integrations/types/{typeId} | Updates an Integration Type.


# **create_integration_type**
> TenantApiIntegrationsV1CreateIntegrationTypeResponse create_integration_type(tenant_api_integrations_v1_create_integration_type_request=tenant_api_integrations_v1_create_integration_type_request)

Creates an Integration Type.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_create_integration_type_request import TenantApiIntegrationsV1CreateIntegrationTypeRequest
from edgraph_platform_client.models.tenant_api_integrations_v1_create_integration_type_response import TenantApiIntegrationsV1CreateIntegrationTypeResponse
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
    api_instance = edgraph_platform_client.IntegrationTypesApi(api_client)
    tenant_api_integrations_v1_create_integration_type_request = edgraph_platform_client.TenantApiIntegrationsV1CreateIntegrationTypeRequest() # TenantApiIntegrationsV1CreateIntegrationTypeRequest |  (optional)

    try:
        # Creates an Integration Type.
        api_response = await api_instance.create_integration_type(tenant_api_integrations_v1_create_integration_type_request=tenant_api_integrations_v1_create_integration_type_request)
        print("The response of IntegrationTypesApi->create_integration_type:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationTypesApi->create_integration_type: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_api_integrations_v1_create_integration_type_request** | [**TenantApiIntegrationsV1CreateIntegrationTypeRequest**](TenantApiIntegrationsV1CreateIntegrationTypeRequest.md)|  | [optional] 

### Return type

[**TenantApiIntegrationsV1CreateIntegrationTypeResponse**](TenantApiIntegrationsV1CreateIntegrationTypeResponse.md)

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

# **delete_integration_type**
> TenantApiIntegrationsV1DeleteIntegrationTypeResponse delete_integration_type(type_id)

Removes an Integration Type.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_delete_integration_type_response import TenantApiIntegrationsV1DeleteIntegrationTypeResponse
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
    api_instance = edgraph_platform_client.IntegrationTypesApi(api_client)
    type_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Removes an Integration Type.
        api_response = await api_instance.delete_integration_type(type_id)
        print("The response of IntegrationTypesApi->delete_integration_type:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationTypesApi->delete_integration_type: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type_id** | **UUID**|  | 

### Return type

[**TenantApiIntegrationsV1DeleteIntegrationTypeResponse**](TenantApiIntegrationsV1DeleteIntegrationTypeResponse.md)

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

# **get_integration_type**
> TenantApiIntegrationsV1GetIntegrationTypeResponse get_integration_type(type_id)

Gets an Integration Type.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_get_integration_type_response import TenantApiIntegrationsV1GetIntegrationTypeResponse
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
    api_instance = edgraph_platform_client.IntegrationTypesApi(api_client)
    type_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets an Integration Type.
        api_response = await api_instance.get_integration_type(type_id)
        print("The response of IntegrationTypesApi->get_integration_type:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationTypesApi->get_integration_type: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type_id** | **UUID**|  | 

### Return type

[**TenantApiIntegrationsV1GetIntegrationTypeResponse**](TenantApiIntegrationsV1GetIntegrationTypeResponse.md)

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

# **search_integration_types**
> TenantApiIntegrationsV1IntegrationTypePaginatedItemsViewModel search_integration_types(page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Search Integration Types.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_integration_type_paginated_items_view_model import TenantApiIntegrationsV1IntegrationTypePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.IntegrationTypesApi(api_client)
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Search Integration Types.
        api_response = await api_instance.search_integration_types(page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of IntegrationTypesApi->search_integration_types:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationTypesApi->search_integration_types: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**TenantApiIntegrationsV1IntegrationTypePaginatedItemsViewModel**](TenantApiIntegrationsV1IntegrationTypePaginatedItemsViewModel.md)

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

# **update_integration_type**
> object update_integration_type(type_id, tenant_api_integrations_v1_update_integration_type_request=tenant_api_integrations_v1_update_integration_type_request)

Updates an Integration Type.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_update_integration_type_request import TenantApiIntegrationsV1UpdateIntegrationTypeRequest
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
    api_instance = edgraph_platform_client.IntegrationTypesApi(api_client)
    type_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    tenant_api_integrations_v1_update_integration_type_request = edgraph_platform_client.TenantApiIntegrationsV1UpdateIntegrationTypeRequest() # TenantApiIntegrationsV1UpdateIntegrationTypeRequest |  (optional)

    try:
        # Updates an Integration Type.
        api_response = await api_instance.update_integration_type(type_id, tenant_api_integrations_v1_update_integration_type_request=tenant_api_integrations_v1_update_integration_type_request)
        print("The response of IntegrationTypesApi->update_integration_type:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationTypesApi->update_integration_type: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type_id** | **UUID**|  | 
 **tenant_api_integrations_v1_update_integration_type_request** | [**TenantApiIntegrationsV1UpdateIntegrationTypeRequest**](TenantApiIntegrationsV1UpdateIntegrationTypeRequest.md)|  | [optional] 

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

