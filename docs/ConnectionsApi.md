# edgraph_platform_client.ConnectionsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**connection_tested_response**](ConnectionsApi.md#connection_tested_response) | **POST** /tenants/{tenantId}/datasync/connections/testconnection | Tests availability of provided connection metadata.
[**create_ed_fi_connection**](ConnectionsApi.md#create_ed_fi_connection) | **POST** /tenants/{tenantId}/edfiadmin/connections | Creates a new Ed-Fi Connection.
[**create_tenant_data_sync_connection**](ConnectionsApi.md#create_tenant_data_sync_connection) | **POST** /tenants/{tenantId}/datasync/connections | Creates a new DataSync connection
[**delete_ed_fi_connection**](ConnectionsApi.md#delete_ed_fi_connection) | **DELETE** /tenants/{tenantId}/edfiadmin/connections/{connectionId} | Deletes an Ed-Fi Connection.
[**delete_tenant_data_sync_connection**](ConnectionsApi.md#delete_tenant_data_sync_connection) | **DELETE** /tenants/{tenantId}/datasync/connections/{connectionId} | Delete a DataSync connection matching the primary key
[**get_all_tenant_data_sync_connections**](ConnectionsApi.md#get_all_tenant_data_sync_connections) | **GET** /tenants/{tenantId}/datasync/connections | Retrieves a list of DataSync Connections
[**get_connection_by_id**](ConnectionsApi.md#get_connection_by_id) | **GET** /tenants/{tenantId}/oneroster/connections/{connectionId} | Retrieves the profile of a Connection.
[**get_ed_fi_connection_by_id**](ConnectionsApi.md#get_ed_fi_connection_by_id) | **GET** /tenants/{tenantId}/edfiadmin/connections/{connectionId} | Retrieves an Ed-Fi Connection by ID.
[**get_ed_fi_connections_async**](ConnectionsApi.md#get_ed_fi_connections_async) | **GET** /tenants/{tenantId}/edfiadmin/connections | Retrieves a list of Ed-Fi Connections.
[**get_ed_fi_ods_backup_codes_descriptors_async**](ConnectionsApi.md#get_ed_fi_ods_backup_codes_descriptors_async) | **GET** /tenants/{tenantId}/edfiadmin/connections/odsbackupcodes | Retrieves a list of Ed-Fi ODS backup codes.
[**get_paged_connections**](ConnectionsApi.md#get_paged_connections) | **GET** /tenants/{tenantId}/oneroster/connections | Retrieves a list of Connections.
[**get_tenant_data_sync_connection_profile_by_id**](ConnectionsApi.md#get_tenant_data_sync_connection_profile_by_id) | **GET** /tenants/{tenantId}/datasync/connections/{connectionId} | Retrieves a specific DataSync connection using its primary key
[**test_connection_details_async**](ConnectionsApi.md#test_connection_details_async) | **POST** /tenants/{tenantId}/oneroster/connections/test | Tests the connection by sending the connection details in the request payload
[**test_connection_details_by_id_async**](ConnectionsApi.md#test_connection_details_by_id_async) | **POST** /tenants/{tenantId}/oneroster/connections/{connectionId}/test | Tests the connection by obtaining the details by ID
[**update_ed_fi_connection**](ConnectionsApi.md#update_ed_fi_connection) | **PUT** /tenants/{tenantId}/edfiadmin/connections/{connectionId} | Updates an Ed-Fi Connection.
[**update_tenant_data_sync_connection**](ConnectionsApi.md#update_tenant_data_sync_connection) | **PUT** /tenants/{tenantId}/datasync/connections/{connectionId} | Updates a DataSync connection matching the primary key


# **connection_tested_response**
> DataSyncApiConnectionV1ConnectionTestedResponse connection_tested_response(tenant_id, data_sync_api_connection_v1_test_connection_request=data_sync_api_connection_v1_test_connection_request)

Tests availability of provided connection metadata.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_connection_v1_connection_tested_response import DataSyncApiConnectionV1ConnectionTestedResponse
from edgraph_platform_client.models.data_sync_api_connection_v1_test_connection_request import DataSyncApiConnectionV1TestConnectionRequest
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
    api_instance = edgraph_platform_client.ConnectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    data_sync_api_connection_v1_test_connection_request = edgraph_platform_client.DataSyncApiConnectionV1TestConnectionRequest() # DataSyncApiConnectionV1TestConnectionRequest |  (optional)

    try:
        # Tests availability of provided connection metadata.
        api_response = await api_instance.connection_tested_response(tenant_id, data_sync_api_connection_v1_test_connection_request=data_sync_api_connection_v1_test_connection_request)
        print("The response of ConnectionsApi->connection_tested_response:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsApi->connection_tested_response: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **data_sync_api_connection_v1_test_connection_request** | [**DataSyncApiConnectionV1TestConnectionRequest**](DataSyncApiConnectionV1TestConnectionRequest.md)|  | [optional] 

### Return type

[**DataSyncApiConnectionV1ConnectionTestedResponse**](DataSyncApiConnectionV1ConnectionTestedResponse.md)

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

# **create_ed_fi_connection**
> create_ed_fi_connection(tenant_id, edfi_admin_api_edfi_admin_v1_create_ed_fi_connection_request=edfi_admin_api_edfi_admin_v1_create_ed_fi_connection_request)

Creates a new Ed-Fi Connection.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_ed_fi_connection_request import EdfiAdminApiEdfiAdminV1CreateEdFiConnectionRequest
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
    api_instance = edgraph_platform_client.ConnectionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    edfi_admin_api_edfi_admin_v1_create_ed_fi_connection_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1CreateEdFiConnectionRequest() # EdfiAdminApiEdfiAdminV1CreateEdFiConnectionRequest |  (optional)

    try:
        # Creates a new Ed-Fi Connection.
        await api_instance.create_ed_fi_connection(tenant_id, edfi_admin_api_edfi_admin_v1_create_ed_fi_connection_request=edfi_admin_api_edfi_admin_v1_create_ed_fi_connection_request)
    except Exception as e:
        print("Exception when calling ConnectionsApi->create_ed_fi_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **edfi_admin_api_edfi_admin_v1_create_ed_fi_connection_request** | [**EdfiAdminApiEdfiAdminV1CreateEdFiConnectionRequest**](EdfiAdminApiEdfiAdminV1CreateEdFiConnectionRequest.md)|  | [optional] 

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
**200** | Success |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**201** | The resource was created. The location of the resource is available in the Location header of the response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_tenant_data_sync_connection**
> create_tenant_data_sync_connection(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_create_connection_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_create_connection_request)

Creates a new DataSync connection

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_create_connection_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsCreateConnectionRequest
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
    api_instance = edgraph_platform_client.ConnectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_create_connection_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsCreateConnectionRequest() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsCreateConnectionRequest |  (optional)

    try:
        # Creates a new DataSync connection
        await api_instance.create_tenant_data_sync_connection(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_create_connection_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_create_connection_request)
    except Exception as e:
        print("Exception when calling ConnectionsApi->create_tenant_data_sync_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_create_connection_request** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsCreateConnectionRequest**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsCreateConnectionRequest.md)|  | [optional] 

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
**201** | The resource was created. The location of the resource is available in the Location header of the response. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_ed_fi_connection**
> EdfiAdminApiEdfiAdminV1EdFiConnectionDeletedResponse delete_ed_fi_connection(tenant_id, connection_id)

Deletes an Ed-Fi Connection.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ed_fi_connection_deleted_response import EdfiAdminApiEdfiAdminV1EdFiConnectionDeletedResponse
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
    api_instance = edgraph_platform_client.ConnectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    connection_id = 'connection_id_example' # str | 

    try:
        # Deletes an Ed-Fi Connection.
        api_response = await api_instance.delete_ed_fi_connection(tenant_id, connection_id)
        print("The response of ConnectionsApi->delete_ed_fi_connection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsApi->delete_ed_fi_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **connection_id** | **str**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1EdFiConnectionDeletedResponse**](EdfiAdminApiEdfiAdminV1EdFiConnectionDeletedResponse.md)

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
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_tenant_data_sync_connection**
> delete_tenant_data_sync_connection(tenant_id, connection_id)

Delete a DataSync connection matching the primary key

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
    api_instance = edgraph_platform_client.ConnectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    connection_id = 'connection_id_example' # str | 

    try:
        # Delete a DataSync connection matching the primary key
        await api_instance.delete_tenant_data_sync_connection(tenant_id, connection_id)
    except Exception as e:
        print("Exception when calling ConnectionsApi->delete_tenant_data_sync_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **connection_id** | **str**|  | 

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

# **get_all_tenant_data_sync_connections**
> DataSyncApiConnectionV1ConnectionListResponsePaginatedItemsViewModel get_all_tenant_data_sync_connections(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of DataSync Connections

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_connection_v1_connection_list_response_paginated_items_view_model import DataSyncApiConnectionV1ConnectionListResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.ConnectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of DataSync Connections
        api_response = await api_instance.get_all_tenant_data_sync_connections(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of ConnectionsApi->get_all_tenant_data_sync_connections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsApi->get_all_tenant_data_sync_connections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**DataSyncApiConnectionV1ConnectionListResponsePaginatedItemsViewModel**](DataSyncApiConnectionV1ConnectionListResponsePaginatedItemsViewModel.md)

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

# **get_connection_by_id**
> IMSAdminApiV1ConnectionsPagedConnectionsResponse get_connection_by_id(tenant_id, connection_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves the profile of a Connection.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_connections_paged_connections_response import IMSAdminApiV1ConnectionsPagedConnectionsResponse
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
    api_instance = edgraph_platform_client.ConnectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    connection_id = 'connection_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves the profile of a Connection.
        api_response = await api_instance.get_connection_by_id(tenant_id, connection_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of ConnectionsApi->get_connection_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsApi->get_connection_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **connection_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**IMSAdminApiV1ConnectionsPagedConnectionsResponse**](IMSAdminApiV1ConnectionsPagedConnectionsResponse.md)

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

# **get_ed_fi_connection_by_id**
> EdfiAdminApiEdfiAdminV1EdFiConnection get_ed_fi_connection_by_id(tenant_id, connection_id)

Retrieves an Ed-Fi Connection by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ed_fi_connection import EdfiAdminApiEdfiAdminV1EdFiConnection
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
    api_instance = edgraph_platform_client.ConnectionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    connection_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Retrieves an Ed-Fi Connection by ID.
        api_response = await api_instance.get_ed_fi_connection_by_id(tenant_id, connection_id)
        print("The response of ConnectionsApi->get_ed_fi_connection_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsApi->get_ed_fi_connection_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **connection_id** | **UUID**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1EdFiConnection**](EdfiAdminApiEdfiAdminV1EdFiConnection.md)

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

# **get_ed_fi_connections_async**
> EdfiAdminApiEdfiAdminV1EdFiConnectionPaginatedItemsResponse get_ed_fi_connections_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of Ed-Fi Connections.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ed_fi_connection_paginated_items_response import EdfiAdminApiEdfiAdminV1EdFiConnectionPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.ConnectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of Ed-Fi Connections.
        api_response = await api_instance.get_ed_fi_connections_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of ConnectionsApi->get_ed_fi_connections_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsApi->get_ed_fi_connections_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdfiAdminApiEdfiAdminV1EdFiConnectionPaginatedItemsResponse**](EdfiAdminApiEdfiAdminV1EdFiConnectionPaginatedItemsResponse.md)

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

# **get_ed_fi_ods_backup_codes_descriptors_async**
> EdfiAdminApiEdfiAdminV1EdFiOdsBackupDescriptorsPaginatedItemsResponse get_ed_fi_ods_backup_codes_descriptors_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of Ed-Fi ODS backup codes.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ed_fi_ods_backup_descriptors_paginated_items_response import EdfiAdminApiEdfiAdminV1EdFiOdsBackupDescriptorsPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.ConnectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of Ed-Fi ODS backup codes.
        api_response = await api_instance.get_ed_fi_ods_backup_codes_descriptors_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of ConnectionsApi->get_ed_fi_ods_backup_codes_descriptors_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsApi->get_ed_fi_ods_backup_codes_descriptors_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdfiAdminApiEdfiAdminV1EdFiOdsBackupDescriptorsPaginatedItemsResponse**](EdfiAdminApiEdfiAdminV1EdFiOdsBackupDescriptorsPaginatedItemsResponse.md)

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

# **get_paged_connections**
> IMSAdminApiV1ConnectionsPagedConnectionsResponse get_paged_connections(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of Connections.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_connections_paged_connections_response import IMSAdminApiV1ConnectionsPagedConnectionsResponse
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
    api_instance = edgraph_platform_client.ConnectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of Connections.
        api_response = await api_instance.get_paged_connections(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of ConnectionsApi->get_paged_connections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsApi->get_paged_connections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**IMSAdminApiV1ConnectionsPagedConnectionsResponse**](IMSAdminApiV1ConnectionsPagedConnectionsResponse.md)

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

# **get_tenant_data_sync_connection_profile_by_id**
> DataSyncApiConnectionV1ConnectionProfileResponse get_tenant_data_sync_connection_profile_by_id(tenant_id, connection_id)

Retrieves a specific DataSync connection using its primary key

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_connection_v1_connection_profile_response import DataSyncApiConnectionV1ConnectionProfileResponse
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
    api_instance = edgraph_platform_client.ConnectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    connection_id = 'connection_id_example' # str | 

    try:
        # Retrieves a specific DataSync connection using its primary key
        api_response = await api_instance.get_tenant_data_sync_connection_profile_by_id(tenant_id, connection_id)
        print("The response of ConnectionsApi->get_tenant_data_sync_connection_profile_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsApi->get_tenant_data_sync_connection_profile_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **connection_id** | **str**|  | 

### Return type

[**DataSyncApiConnectionV1ConnectionProfileResponse**](DataSyncApiConnectionV1ConnectionProfileResponse.md)

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

# **test_connection_details_async**
> IMSAdminApiV1ConnectionsConnectionTestedResponse test_connection_details_async(tenant_id, ims_admin_api_v1_connections_test_connection_details_request=ims_admin_api_v1_connections_test_connection_details_request)

Tests the connection by sending the connection details in the request payload

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_connections_connection_tested_response import IMSAdminApiV1ConnectionsConnectionTestedResponse
from edgraph_platform_client.models.ims_admin_api_v1_connections_test_connection_details_request import IMSAdminApiV1ConnectionsTestConnectionDetailsRequest
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
    api_instance = edgraph_platform_client.ConnectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ims_admin_api_v1_connections_test_connection_details_request = edgraph_platform_client.IMSAdminApiV1ConnectionsTestConnectionDetailsRequest() # IMSAdminApiV1ConnectionsTestConnectionDetailsRequest |  (optional)

    try:
        # Tests the connection by sending the connection details in the request payload
        api_response = await api_instance.test_connection_details_async(tenant_id, ims_admin_api_v1_connections_test_connection_details_request=ims_admin_api_v1_connections_test_connection_details_request)
        print("The response of ConnectionsApi->test_connection_details_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsApi->test_connection_details_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ims_admin_api_v1_connections_test_connection_details_request** | [**IMSAdminApiV1ConnectionsTestConnectionDetailsRequest**](IMSAdminApiV1ConnectionsTestConnectionDetailsRequest.md)|  | [optional] 

### Return type

[**IMSAdminApiV1ConnectionsConnectionTestedResponse**](IMSAdminApiV1ConnectionsConnectionTestedResponse.md)

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

# **test_connection_details_by_id_async**
> IMSAdminApiV1ConnectionsConnectionTestedResponse test_connection_details_by_id_async(tenant_id, connection_id, ims_admin_api_v1_connections_test_connection_details_by_id_request=ims_admin_api_v1_connections_test_connection_details_by_id_request)

Tests the connection by obtaining the details by ID

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_connections_connection_tested_response import IMSAdminApiV1ConnectionsConnectionTestedResponse
from edgraph_platform_client.models.ims_admin_api_v1_connections_test_connection_details_by_id_request import IMSAdminApiV1ConnectionsTestConnectionDetailsByIdRequest
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
    api_instance = edgraph_platform_client.ConnectionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    connection_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ims_admin_api_v1_connections_test_connection_details_by_id_request = edgraph_platform_client.IMSAdminApiV1ConnectionsTestConnectionDetailsByIdRequest() # IMSAdminApiV1ConnectionsTestConnectionDetailsByIdRequest |  (optional)

    try:
        # Tests the connection by obtaining the details by ID
        api_response = await api_instance.test_connection_details_by_id_async(tenant_id, connection_id, ims_admin_api_v1_connections_test_connection_details_by_id_request=ims_admin_api_v1_connections_test_connection_details_by_id_request)
        print("The response of ConnectionsApi->test_connection_details_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsApi->test_connection_details_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **connection_id** | **UUID**|  | 
 **ims_admin_api_v1_connections_test_connection_details_by_id_request** | [**IMSAdminApiV1ConnectionsTestConnectionDetailsByIdRequest**](IMSAdminApiV1ConnectionsTestConnectionDetailsByIdRequest.md)|  | [optional] 

### Return type

[**IMSAdminApiV1ConnectionsConnectionTestedResponse**](IMSAdminApiV1ConnectionsConnectionTestedResponse.md)

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

# **update_ed_fi_connection**
> EdfiAdminApiEdfiAdminV1EdFiConnectionUpdatedResponse update_ed_fi_connection(tenant_id, connection_id, edfi_admin_api_edfi_admin_v1_update_ed_fi_connection_request=edfi_admin_api_edfi_admin_v1_update_ed_fi_connection_request)

Updates an Ed-Fi Connection.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ed_fi_connection_updated_response import EdfiAdminApiEdfiAdminV1EdFiConnectionUpdatedResponse
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_ed_fi_connection_request import EdfiAdminApiEdfiAdminV1UpdateEdFiConnectionRequest
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
    api_instance = edgraph_platform_client.ConnectionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    connection_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    edfi_admin_api_edfi_admin_v1_update_ed_fi_connection_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1UpdateEdFiConnectionRequest() # EdfiAdminApiEdfiAdminV1UpdateEdFiConnectionRequest |  (optional)

    try:
        # Updates an Ed-Fi Connection.
        api_response = await api_instance.update_ed_fi_connection(tenant_id, connection_id, edfi_admin_api_edfi_admin_v1_update_ed_fi_connection_request=edfi_admin_api_edfi_admin_v1_update_ed_fi_connection_request)
        print("The response of ConnectionsApi->update_ed_fi_connection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsApi->update_ed_fi_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **connection_id** | **UUID**|  | 
 **edfi_admin_api_edfi_admin_v1_update_ed_fi_connection_request** | [**EdfiAdminApiEdfiAdminV1UpdateEdFiConnectionRequest**](EdfiAdminApiEdfiAdminV1UpdateEdFiConnectionRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1EdFiConnectionUpdatedResponse**](EdfiAdminApiEdfiAdminV1EdFiConnectionUpdatedResponse.md)

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
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_tenant_data_sync_connection**
> update_tenant_data_sync_connection(tenant_id, connection_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_update_connection_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_update_connection_request)

Updates a DataSync connection matching the primary key

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_update_connection_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsUpdateConnectionRequest
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
    api_instance = edgraph_platform_client.ConnectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    connection_id = 'connection_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_update_connection_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsUpdateConnectionRequest() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsUpdateConnectionRequest |  (optional)

    try:
        # Updates a DataSync connection matching the primary key
        await api_instance.update_tenant_data_sync_connection(tenant_id, connection_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_update_connection_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_update_connection_request)
    except Exception as e:
        print("Exception when calling ConnectionsApi->update_tenant_data_sync_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **connection_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_update_connection_request** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsUpdateConnectionRequest**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsUpdateConnectionRequest.md)|  | [optional] 

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

