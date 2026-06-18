# edgraph_platform_client.InstancesClientsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_client**](InstancesClientsApi.md#create_client) | **POST** /tenants/{tenantId}/oneroster/instances/{instanceId}/clients | Creates a new client
[**delete_client**](InstancesClientsApi.md#delete_client) | **DELETE** /tenants/{tenantId}/oneroster/instances/{instanceId}/clients/{clientId} | Deletes a client by Id
[**get_client_by_id**](InstancesClientsApi.md#get_client_by_id) | **GET** /tenants/{tenantId}/oneroster/instances/{instanceId}/clients/{clientId} | Retrieves a client by Id
[**get_paged_clients**](InstancesClientsApi.md#get_paged_clients) | **GET** /tenants/{tenantId}/oneroster/instances/{instanceId}/clients | Retrieves a list of clients for a given instance
[**update_client**](InstancesClientsApi.md#update_client) | **PUT** /tenants/{tenantId}/oneroster/instances/{instanceId}/clients/{clientId} | Updates a client by Id


# **create_client**
> IMSAdminApiV1ClientsClientCreatedResponse create_client(tenant_id, instance_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_one_roster_create_client_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_one_roster_create_client_request_dto)

Creates a new client

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_one_roster_create_client_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsOneRosterCreateClientRequestDto
from edgraph_platform_client.models.ims_admin_api_v1_clients_client_created_response import IMSAdminApiV1ClientsClientCreatedResponse
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
    api_instance = edgraph_platform_client.InstancesClientsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_one_roster_create_client_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsOneRosterCreateClientRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsOneRosterCreateClientRequestDto |  (optional)

    try:
        # Creates a new client
        api_response = await api_instance.create_client(tenant_id, instance_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_one_roster_create_client_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_one_roster_create_client_request_dto)
        print("The response of InstancesClientsApi->create_client:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesClientsApi->create_client: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_one_roster_create_client_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsOneRosterCreateClientRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsOneRosterCreateClientRequestDto.md)|  | [optional] 

### Return type

[**IMSAdminApiV1ClientsClientCreatedResponse**](IMSAdminApiV1ClientsClientCreatedResponse.md)

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

# **delete_client**
> IMSAdminApiV1ClientsClientDeletedResponse delete_client(tenant_id, instance_id, client_id)

Deletes a client by Id

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_clients_client_deleted_response import IMSAdminApiV1ClientsClientDeletedResponse
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
    api_instance = edgraph_platform_client.InstancesClientsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    client_id = 'client_id_example' # str | 

    try:
        # Deletes a client by Id
        api_response = await api_instance.delete_client(tenant_id, instance_id, client_id)
        print("The response of InstancesClientsApi->delete_client:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesClientsApi->delete_client: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **client_id** | **str**|  | 

### Return type

[**IMSAdminApiV1ClientsClientDeletedResponse**](IMSAdminApiV1ClientsClientDeletedResponse.md)

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

# **get_client_by_id**
> IMSAdminApiV1ClientsClientProfileResponse get_client_by_id(tenant_id, instance_id, client_id)

Retrieves a client by Id

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_clients_client_profile_response import IMSAdminApiV1ClientsClientProfileResponse
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
    api_instance = edgraph_platform_client.InstancesClientsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    client_id = 'client_id_example' # str | 

    try:
        # Retrieves a client by Id
        api_response = await api_instance.get_client_by_id(tenant_id, instance_id, client_id)
        print("The response of InstancesClientsApi->get_client_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesClientsApi->get_client_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **client_id** | **str**|  | 

### Return type

[**IMSAdminApiV1ClientsClientProfileResponse**](IMSAdminApiV1ClientsClientProfileResponse.md)

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

# **get_paged_clients**
> IMSAdminApiV1ClientsPaginatedItemsResponse get_paged_clients(tenant_id, instance_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of clients for a given instance

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_clients_paginated_items_response import IMSAdminApiV1ClientsPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.InstancesClientsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of clients for a given instance
        api_response = await api_instance.get_paged_clients(tenant_id, instance_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of InstancesClientsApi->get_paged_clients:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesClientsApi->get_paged_clients: %s\n" % e)
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

[**IMSAdminApiV1ClientsPaginatedItemsResponse**](IMSAdminApiV1ClientsPaginatedItemsResponse.md)

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

# **update_client**
> IMSAdminApiV1ClientsClientUpdatedResponse update_client(tenant_id, instance_id, client_id, ims_admin_api_v1_clients_update_client_request=ims_admin_api_v1_clients_update_client_request)

Updates a client by Id

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_clients_client_updated_response import IMSAdminApiV1ClientsClientUpdatedResponse
from edgraph_platform_client.models.ims_admin_api_v1_clients_update_client_request import IMSAdminApiV1ClientsUpdateClientRequest
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
    api_instance = edgraph_platform_client.InstancesClientsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    client_id = 'client_id_example' # str | 
    ims_admin_api_v1_clients_update_client_request = edgraph_platform_client.IMSAdminApiV1ClientsUpdateClientRequest() # IMSAdminApiV1ClientsUpdateClientRequest |  (optional)

    try:
        # Updates a client by Id
        api_response = await api_instance.update_client(tenant_id, instance_id, client_id, ims_admin_api_v1_clients_update_client_request=ims_admin_api_v1_clients_update_client_request)
        print("The response of InstancesClientsApi->update_client:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesClientsApi->update_client: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **client_id** | **str**|  | 
 **ims_admin_api_v1_clients_update_client_request** | [**IMSAdminApiV1ClientsUpdateClientRequest**](IMSAdminApiV1ClientsUpdateClientRequest.md)|  | [optional] 

### Return type

[**IMSAdminApiV1ClientsClientUpdatedResponse**](IMSAdminApiV1ClientsClientUpdatedResponse.md)

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

