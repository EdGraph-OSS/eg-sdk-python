# edgraph_platform_client.EnvironmentsConnectionsByTypeApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_or_update_state_reporting_connection_by_type**](EnvironmentsConnectionsByTypeApi.md#create_or_update_state_reporting_connection_by_type) | **PUT** /tenants/{tenantId}/statereporting/environments/{environmentId}/connectionsByType/{connectionType} | Creates or Update a Connection by ConnectionType.
[**delete_state_reporting_by_type_connection**](EnvironmentsConnectionsByTypeApi.md#delete_state_reporting_by_type_connection) | **DELETE** /tenants/{tenantId}/statereporting/environments/{environmentId}/connectionsByType/{connectionType} | Deletes a Connection by Type
[**get_state_reporting_connection_by_type**](EnvironmentsConnectionsByTypeApi.md#get_state_reporting_connection_by_type) | **GET** /tenants/{tenantId}/statereporting/environments/{environmentId}/connectionsByType/{connectionType} | Retrieves a Connection by Type.


# **create_or_update_state_reporting_connection_by_type**
> EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionCreatedResponse create_or_update_state_reporting_connection_by_type(tenant_id, environment_id, connection_type, ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_create_connection_request=ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_create_connection_request)

Creates or Update a Connection by ConnectionType.

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
    api_instance = edgraph_platform_client.EnvironmentsConnectionsByTypeApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    connection_type = 'connection_type_example' # str | 
    ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_create_connection_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesStateReportingV1CreateConnectionRequest() # EdGraphHttpAggregatorsTenantApiServicesStateReportingV1CreateConnectionRequest |  (optional)

    try:
        # Creates or Update a Connection by ConnectionType.
        api_response = await api_instance.create_or_update_state_reporting_connection_by_type(tenant_id, environment_id, connection_type, ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_create_connection_request=ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_create_connection_request)
        print("The response of EnvironmentsConnectionsByTypeApi->create_or_update_state_reporting_connection_by_type:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsConnectionsByTypeApi->create_or_update_state_reporting_connection_by_type: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **connection_type** | **str**|  | 
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

# **delete_state_reporting_by_type_connection**
> EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionDeletedResponse delete_state_reporting_by_type_connection(tenant_id, environment_id, connection_type)

Deletes a Connection by Type

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
    api_instance = edgraph_platform_client.EnvironmentsConnectionsByTypeApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    connection_type = 'connection_type_example' # str | 

    try:
        # Deletes a Connection by Type
        api_response = await api_instance.delete_state_reporting_by_type_connection(tenant_id, environment_id, connection_type)
        print("The response of EnvironmentsConnectionsByTypeApi->delete_state_reporting_by_type_connection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsConnectionsByTypeApi->delete_state_reporting_by_type_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **connection_type** | **str**|  | 

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

# **get_state_reporting_connection_by_type**
> EdGraphHttpAggregatorsTenantApiServicesStateReportingV1ConnectionProfileResponse get_state_reporting_connection_by_type(tenant_id, environment_id, connection_type)

Retrieves a Connection by Type.

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
    api_instance = edgraph_platform_client.EnvironmentsConnectionsByTypeApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    connection_type = 'connection_type_example' # str | 

    try:
        # Retrieves a Connection by Type.
        api_response = await api_instance.get_state_reporting_connection_by_type(tenant_id, environment_id, connection_type)
        print("The response of EnvironmentsConnectionsByTypeApi->get_state_reporting_connection_by_type:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsConnectionsByTypeApi->get_state_reporting_connection_by_type: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **connection_type** | **str**|  | 

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

