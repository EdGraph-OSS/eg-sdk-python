# edgraph_platform_client.TenantIntegrationsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_tenant_integration**](TenantIntegrationsApi.md#add_tenant_integration) | **POST** /tenants/{tenantId}/integrations | Creates an Integration for a tenant.
[**delete_tenant_integration**](TenantIntegrationsApi.md#delete_tenant_integration) | **DELETE** /tenants/{tenantId}/integrations/{id} | Removes a tenant Integration.
[**get_tenant_integration**](TenantIntegrationsApi.md#get_tenant_integration) | **GET** /tenants/{tenantId}/integrations/{id} | Gets a tenant Integration.
[**search_integrations**](TenantIntegrationsApi.md#search_integrations) | **GET** /tenants/{tenantId}/integrations | Search a Tenant&#39;s Integrations
[**update_tenant_integration**](TenantIntegrationsApi.md#update_tenant_integration) | **PUT** /tenants/{tenantId}/integrations/{id} | Updates a tenant Integration.


# **add_tenant_integration**
> TenantApiIntegrationsV1CreateIntegrationResponse add_tenant_integration(tenant_id, tenant_api_integrations_v1_create_integration_request=tenant_api_integrations_v1_create_integration_request)

Creates an Integration for a tenant.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_create_integration_request import TenantApiIntegrationsV1CreateIntegrationRequest
from edgraph_platform_client.models.tenant_api_integrations_v1_create_integration_response import TenantApiIntegrationsV1CreateIntegrationResponse
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
    api_instance = edgraph_platform_client.TenantIntegrationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    tenant_api_integrations_v1_create_integration_request = edgraph_platform_client.TenantApiIntegrationsV1CreateIntegrationRequest() # TenantApiIntegrationsV1CreateIntegrationRequest |  (optional)

    try:
        # Creates an Integration for a tenant.
        api_response = await api_instance.add_tenant_integration(tenant_id, tenant_api_integrations_v1_create_integration_request=tenant_api_integrations_v1_create_integration_request)
        print("The response of TenantIntegrationsApi->add_tenant_integration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantIntegrationsApi->add_tenant_integration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **tenant_api_integrations_v1_create_integration_request** | [**TenantApiIntegrationsV1CreateIntegrationRequest**](TenantApiIntegrationsV1CreateIntegrationRequest.md)|  | [optional] 

### Return type

[**TenantApiIntegrationsV1CreateIntegrationResponse**](TenantApiIntegrationsV1CreateIntegrationResponse.md)

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
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_tenant_integration**
> TenantApiIntegrationsV1DeleteIntegrationResponse delete_tenant_integration(tenant_id, id)

Removes a tenant Integration.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_delete_integration_response import TenantApiIntegrationsV1DeleteIntegrationResponse
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
    api_instance = edgraph_platform_client.TenantIntegrationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Removes a tenant Integration.
        api_response = await api_instance.delete_tenant_integration(tenant_id, id)
        print("The response of TenantIntegrationsApi->delete_tenant_integration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantIntegrationsApi->delete_tenant_integration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **id** | **UUID**|  | 

### Return type

[**TenantApiIntegrationsV1DeleteIntegrationResponse**](TenantApiIntegrationsV1DeleteIntegrationResponse.md)

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
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_tenant_integration**
> TenantApiIntegrationsV1GetIntegrationResponse get_tenant_integration(tenant_id, id)

Gets a tenant Integration.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_get_integration_response import TenantApiIntegrationsV1GetIntegrationResponse
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
    api_instance = edgraph_platform_client.TenantIntegrationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets a tenant Integration.
        api_response = await api_instance.get_tenant_integration(tenant_id, id)
        print("The response of TenantIntegrationsApi->get_tenant_integration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantIntegrationsApi->get_tenant_integration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **id** | **UUID**|  | 

### Return type

[**TenantApiIntegrationsV1GetIntegrationResponse**](TenantApiIntegrationsV1GetIntegrationResponse.md)

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
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **search_integrations**
> TenantApiIntegrationsV1IntegrationPaginatedItemsViewModel search_integrations(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Search a Tenant's Integrations

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_integration_paginated_items_view_model import TenantApiIntegrationsV1IntegrationPaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.TenantIntegrationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Search a Tenant's Integrations
        api_response = await api_instance.search_integrations(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of TenantIntegrationsApi->search_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantIntegrationsApi->search_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**TenantApiIntegrationsV1IntegrationPaginatedItemsViewModel**](TenantApiIntegrationsV1IntegrationPaginatedItemsViewModel.md)

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_tenant_integration**
> object update_tenant_integration(tenant_id, id, tenant_api_integrations_v1_update_integration_request=tenant_api_integrations_v1_update_integration_request)

Updates a tenant Integration.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_update_integration_request import TenantApiIntegrationsV1UpdateIntegrationRequest
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
    api_instance = edgraph_platform_client.TenantIntegrationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    tenant_api_integrations_v1_update_integration_request = edgraph_platform_client.TenantApiIntegrationsV1UpdateIntegrationRequest() # TenantApiIntegrationsV1UpdateIntegrationRequest |  (optional)

    try:
        # Updates a tenant Integration.
        api_response = await api_instance.update_tenant_integration(tenant_id, id, tenant_api_integrations_v1_update_integration_request=tenant_api_integrations_v1_update_integration_request)
        print("The response of TenantIntegrationsApi->update_tenant_integration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantIntegrationsApi->update_tenant_integration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **id** | **UUID**|  | 
 **tenant_api_integrations_v1_update_integration_request** | [**TenantApiIntegrationsV1UpdateIntegrationRequest**](TenantApiIntegrationsV1UpdateIntegrationRequest.md)|  | [optional] 

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
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

