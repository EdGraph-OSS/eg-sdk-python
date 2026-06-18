# edgraph_platform_client.EnvironmentsConnectionsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_state_reporting_connection**](EnvironmentsConnectionsApi.md#create_state_reporting_connection) | **POST** /tenants/{tenantId}/statereporting/environments/{environmentId}/connections | Creates a new Connection.
[**delete_state_reporting_connection**](EnvironmentsConnectionsApi.md#delete_state_reporting_connection) | **DELETE** /tenants/{tenantId}/statereporting/environments/{environmentId}/connections/{connectionId} | Deletes a Connection.
[**find_state_reporting_connections**](EnvironmentsConnectionsApi.md#find_state_reporting_connections) | **GET** /tenants/{tenantId}/statereporting/environments/{environmentId}/connections | Retrieves a list of Connections.
[**get_state_reporting_connection**](EnvironmentsConnectionsApi.md#get_state_reporting_connection) | **GET** /tenants/{tenantId}/statereporting/environments/{environmentId}/connections/{connectionId} | Retrieves a Connection by ID.
[**test_state_reporting_connection_by_id**](EnvironmentsConnectionsApi.md#test_state_reporting_connection_by_id) | **POST** /tenants/{tenantId}/statereporting/environments/{environmentId}/connections/{connectionId}/testconnection | Tests a Connection by ID.
[**test_state_reporting_connection_by_type**](EnvironmentsConnectionsApi.md#test_state_reporting_connection_by_type) | **POST** /tenants/{tenantId}/statereporting/environments/{environmentId}/connections/testconnection | Tests a Connection by Type.
[**update_state_reporting_connection**](EnvironmentsConnectionsApi.md#update_state_reporting_connection) | **PUT** /tenants/{tenantId}/statereporting/environments/{environmentId}/connections/{connectionId} | Updates a Connection.


# **create_state_reporting_connection**
> EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionCreatedResponse create_state_reporting_connection(tenant_id, environment_id, ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_create_connection_request=ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_create_connection_request)

Creates a new Connection.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_connection_created_response import EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionCreatedResponse
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_create_connection_request import EdGraphHttpAggregatorsTenantApiServicesStateReportingV1CreateConnectionRequest
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
    api_instance = edgraph_platform_client.EnvironmentsConnectionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_create_connection_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesStateReportingV1CreateConnectionRequest() # EdGraphHttpAggregatorsTenantApiServicesStateReportingV1CreateConnectionRequest |  (optional)

    try:
        # Creates a new Connection.
        api_response = await api_instance.create_state_reporting_connection(tenant_id, environment_id, ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_create_connection_request=ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_create_connection_request)
        print("The response of EnvironmentsConnectionsApi->create_state_reporting_connection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsConnectionsApi->create_state_reporting_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_create_connection_request** | [**EdGraphHttpAggregatorsTenantApiServicesStateReportingV1CreateConnectionRequest**](EdGraphHttpAggregatorsTenantApiServicesStateReportingV1CreateConnectionRequest.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionCreatedResponse**](EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionCreatedResponse.md)

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

# **delete_state_reporting_connection**
> EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionDeletedResponse delete_state_reporting_connection(tenant_id, environment_id, connection_id)

Deletes a Connection.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_connection_deleted_response import EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionDeletedResponse
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
    api_instance = edgraph_platform_client.EnvironmentsConnectionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    connection_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Deletes a Connection.
        api_response = await api_instance.delete_state_reporting_connection(tenant_id, environment_id, connection_id)
        print("The response of EnvironmentsConnectionsApi->delete_state_reporting_connection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsConnectionsApi->delete_state_reporting_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **connection_id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionDeletedResponse**](EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionDeletedResponse.md)

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

# **find_state_reporting_connections**
> EdGraphHttpAggregatorsTenantApiServicesStateReportingV1PagedConnectionsResponse find_state_reporting_connections(tenant_id, environment_id, instance_type=instance_type, connection_type=connection_type)

Retrieves a list of Connections.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_paged_connections_response import EdGraphHttpAggregatorsTenantApiServicesStateReportingV1PagedConnectionsResponse
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
    api_instance = edgraph_platform_client.EnvironmentsConnectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    instance_type = 'instance_type_example' # str |  (optional)
    connection_type = 'connection_type_example' # str |  (optional)

    try:
        # Retrieves a list of Connections.
        api_response = await api_instance.find_state_reporting_connections(tenant_id, environment_id, instance_type=instance_type, connection_type=connection_type)
        print("The response of EnvironmentsConnectionsApi->find_state_reporting_connections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsConnectionsApi->find_state_reporting_connections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **UUID**|  | 
 **instance_type** | **str**|  | [optional] 
 **connection_type** | **str**|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesStateReportingV1PagedConnectionsResponse**](EdGraphHttpAggregatorsTenantApiServicesStateReportingV1PagedConnectionsResponse.md)

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

# **get_state_reporting_connection**
> EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionProfileResponse get_state_reporting_connection(tenant_id, environment_id, connection_id)

Retrieves a Connection by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_connection_profile_response import EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionProfileResponse
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
    api_instance = edgraph_platform_client.EnvironmentsConnectionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    connection_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Retrieves a Connection by ID.
        api_response = await api_instance.get_state_reporting_connection(tenant_id, environment_id, connection_id)
        print("The response of EnvironmentsConnectionsApi->get_state_reporting_connection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsConnectionsApi->get_state_reporting_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **connection_id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionProfileResponse**](EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionProfileResponse.md)

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

# **test_state_reporting_connection_by_id**
> EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionResponse test_state_reporting_connection_by_id(tenant_id, environment_id, connection_id)

Tests a Connection by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_test_connection_response import EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionResponse
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
    api_instance = edgraph_platform_client.EnvironmentsConnectionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    connection_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Tests a Connection by ID.
        api_response = await api_instance.test_state_reporting_connection_by_id(tenant_id, environment_id, connection_id)
        print("The response of EnvironmentsConnectionsApi->test_state_reporting_connection_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsConnectionsApi->test_state_reporting_connection_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **connection_id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionResponse**](EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionResponse.md)

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

# **test_state_reporting_connection_by_type**
> EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionResponse test_state_reporting_connection_by_type(tenant_id, environment_id, ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_test_connection_by_type_request=ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_test_connection_by_type_request)

Tests a Connection by Type.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_test_connection_by_type_request import EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionByTypeRequest
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_test_connection_response import EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionResponse
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
    api_instance = edgraph_platform_client.EnvironmentsConnectionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_test_connection_by_type_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionByTypeRequest() # EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionByTypeRequest |  (optional)

    try:
        # Tests a Connection by Type.
        api_response = await api_instance.test_state_reporting_connection_by_type(tenant_id, environment_id, ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_test_connection_by_type_request=ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_test_connection_by_type_request)
        print("The response of EnvironmentsConnectionsApi->test_state_reporting_connection_by_type:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsConnectionsApi->test_state_reporting_connection_by_type: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_test_connection_by_type_request** | [**EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionByTypeRequest**](EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionByTypeRequest.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionResponse**](EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionResponse.md)

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

# **update_state_reporting_connection**
> EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionUpdatedResponse update_state_reporting_connection(tenant_id, environment_id, connection_id, ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_update_connection_request=ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_update_connection_request)

Updates a Connection.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_connection_updated_response import EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionUpdatedResponse
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_update_connection_request import EdGraphHttpAggregatorsTenantApiServicesStateReportingV1UpdateConnectionRequest
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
    api_instance = edgraph_platform_client.EnvironmentsConnectionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    connection_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_update_connection_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesStateReportingV1UpdateConnectionRequest() # EdGraphHttpAggregatorsTenantApiServicesStateReportingV1UpdateConnectionRequest |  (optional)

    try:
        # Updates a Connection.
        api_response = await api_instance.update_state_reporting_connection(tenant_id, environment_id, connection_id, ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_update_connection_request=ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_update_connection_request)
        print("The response of EnvironmentsConnectionsApi->update_state_reporting_connection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsConnectionsApi->update_state_reporting_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **connection_id** | **UUID**|  | 
 **ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_update_connection_request** | [**EdGraphHttpAggregatorsTenantApiServicesStateReportingV1UpdateConnectionRequest**](EdGraphHttpAggregatorsTenantApiServicesStateReportingV1UpdateConnectionRequest.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionUpdatedResponse**](EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionUpdatedResponse.md)

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

