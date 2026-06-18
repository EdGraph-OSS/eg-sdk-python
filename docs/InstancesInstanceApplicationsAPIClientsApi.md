# edgraph_platform_client.InstancesInstanceApplicationsAPIClientsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_instance_api_client**](InstancesInstanceApplicationsAPIClientsApi.md#create_instance_api_client) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/instanceapplications/{applicationId}/apiclients | Creates an Instance ApiClient
[**delete_instance_api_client**](InstancesInstanceApplicationsAPIClientsApi.md#delete_instance_api_client) | **DELETE** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/instanceapplications/{applicationId}/apiclients/{apiClientId} | Deletes an Instance ApiClient
[**get_instance_api_client_by_id**](InstancesInstanceApplicationsAPIClientsApi.md#get_instance_api_client_by_id) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/instanceapplications/{applicationId}/apiclients/{apiClientId} | Retrieves an Instance ApiClient by ID.
[**get_instance_api_clients**](InstancesInstanceApplicationsAPIClientsApi.md#get_instance_api_clients) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/instanceapplications/{applicationId}/apiclients | Retrieves a paginated list of Instance ApiClients
[**update_instance_api_client**](InstancesInstanceApplicationsAPIClientsApi.md#update_instance_api_client) | **PUT** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/instanceapplications/{applicationId}/apiclients/{apiClientId} | Updates an Instance Application ApiClient


# **create_instance_api_client**
> EdfiAdminApiEdfiAdminV1InstanceApiClientCreatedResponse create_instance_api_client(tenant_id, instance_id, application_id, edfi_admin_api_edfi_admin_v1_create_instance_api_client_request=edfi_admin_api_edfi_admin_v1_create_instance_api_client_request)

Creates an Instance ApiClient

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_instance_api_client_request import EdfiAdminApiEdfiAdminV1CreateInstanceApiClientRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_api_client_created_response import EdfiAdminApiEdfiAdminV1InstanceApiClientCreatedResponse
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
    api_instance = edgraph_platform_client.InstancesInstanceApplicationsAPIClientsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 'application_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_create_instance_api_client_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1CreateInstanceApiClientRequest() # EdfiAdminApiEdfiAdminV1CreateInstanceApiClientRequest |  (optional)

    try:
        # Creates an Instance ApiClient
        api_response = await api_instance.create_instance_api_client(tenant_id, instance_id, application_id, edfi_admin_api_edfi_admin_v1_create_instance_api_client_request=edfi_admin_api_edfi_admin_v1_create_instance_api_client_request)
        print("The response of InstancesInstanceApplicationsAPIClientsApi->create_instance_api_client:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesInstanceApplicationsAPIClientsApi->create_instance_api_client: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_create_instance_api_client_request** | [**EdfiAdminApiEdfiAdminV1CreateInstanceApiClientRequest**](EdfiAdminApiEdfiAdminV1CreateInstanceApiClientRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1InstanceApiClientCreatedResponse**](EdfiAdminApiEdfiAdminV1InstanceApiClientCreatedResponse.md)

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_instance_api_client**
> delete_instance_api_client(tenant_id, instance_id, application_id, api_client_id)

Deletes an Instance ApiClient

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
    api_instance = edgraph_platform_client.InstancesInstanceApplicationsAPIClientsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 'application_id_example' # str | 
    api_client_id = 'api_client_id_example' # str | 

    try:
        # Deletes an Instance ApiClient
        await api_instance.delete_instance_api_client(tenant_id, instance_id, application_id, api_client_id)
    except Exception as e:
        print("Exception when calling InstancesInstanceApplicationsAPIClientsApi->delete_instance_api_client: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **str**|  | 
 **api_client_id** | **str**|  | 

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

# **get_instance_api_client_by_id**
> EdfiAdminApiEdfiAdminV1InstanceApiClientProfileResponse get_instance_api_client_by_id(tenant_id, instance_id, application_id, api_client_id)

Retrieves an Instance ApiClient by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_api_client_profile_response import EdfiAdminApiEdfiAdminV1InstanceApiClientProfileResponse
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
    api_instance = edgraph_platform_client.InstancesInstanceApplicationsAPIClientsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 'application_id_example' # str | 
    api_client_id = 'api_client_id_example' # str | 

    try:
        # Retrieves an Instance ApiClient by ID.
        api_response = await api_instance.get_instance_api_client_by_id(tenant_id, instance_id, application_id, api_client_id)
        print("The response of InstancesInstanceApplicationsAPIClientsApi->get_instance_api_client_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesInstanceApplicationsAPIClientsApi->get_instance_api_client_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **str**|  | 
 **api_client_id** | **str**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1InstanceApiClientProfileResponse**](EdfiAdminApiEdfiAdminV1InstanceApiClientProfileResponse.md)

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

# **get_instance_api_clients**
> EdfiAdminApiEdfiAdminV1InstanceApiClientListResponsePaginatedItemsViewModel get_instance_api_clients(tenant_id, instance_id, application_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a paginated list of Instance ApiClients

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_api_client_list_response_paginated_items_view_model import EdfiAdminApiEdfiAdminV1InstanceApiClientListResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.InstancesInstanceApplicationsAPIClientsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 'application_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a paginated list of Instance ApiClients
        api_response = await api_instance.get_instance_api_clients(tenant_id, instance_id, application_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of InstancesInstanceApplicationsAPIClientsApi->get_instance_api_clients:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesInstanceApplicationsAPIClientsApi->get_instance_api_clients: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdfiAdminApiEdfiAdminV1InstanceApiClientListResponsePaginatedItemsViewModel**](EdfiAdminApiEdfiAdminV1InstanceApiClientListResponsePaginatedItemsViewModel.md)

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

# **update_instance_api_client**
> EdfiAdminApiEdfiAdminV1InstanceApiClientUpdatedResponse update_instance_api_client(tenant_id, instance_id, application_id, api_client_id, edfi_admin_api_edfi_admin_v1_update_instance_api_client_request=edfi_admin_api_edfi_admin_v1_update_instance_api_client_request)

Updates an Instance Application ApiClient

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_api_client_updated_response import EdfiAdminApiEdfiAdminV1InstanceApiClientUpdatedResponse
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_instance_api_client_request import EdfiAdminApiEdfiAdminV1UpdateInstanceApiClientRequest
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
    api_instance = edgraph_platform_client.InstancesInstanceApplicationsAPIClientsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 'application_id_example' # str | 
    api_client_id = 'api_client_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_update_instance_api_client_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1UpdateInstanceApiClientRequest() # EdfiAdminApiEdfiAdminV1UpdateInstanceApiClientRequest |  (optional)

    try:
        # Updates an Instance Application ApiClient
        api_response = await api_instance.update_instance_api_client(tenant_id, instance_id, application_id, api_client_id, edfi_admin_api_edfi_admin_v1_update_instance_api_client_request=edfi_admin_api_edfi_admin_v1_update_instance_api_client_request)
        print("The response of InstancesInstanceApplicationsAPIClientsApi->update_instance_api_client:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesInstanceApplicationsAPIClientsApi->update_instance_api_client: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **str**|  | 
 **api_client_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_update_instance_api_client_request** | [**EdfiAdminApiEdfiAdminV1UpdateInstanceApiClientRequest**](EdfiAdminApiEdfiAdminV1UpdateInstanceApiClientRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1InstanceApiClientUpdatedResponse**](EdfiAdminApiEdfiAdminV1InstanceApiClientUpdatedResponse.md)

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

