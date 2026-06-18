# edgraph_platform_client.ConnectionsEdFiApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_tenant_data_sync_connection_ed_fi_districts**](ConnectionsEdFiApi.md#get_tenant_data_sync_connection_ed_fi_districts) | **GET** /tenants/{tenantId}/datasync/connections/{connectionId}/edfi/districts | Retrieves a list of districts from an Ed-Fi API using the DataSync connection metadata
[**get_tenant_data_sync_connection_ed_fi_education_organization_id_descriptors**](ConnectionsEdFiApi.md#get_tenant_data_sync_connection_ed_fi_education_organization_id_descriptors) | **GET** /tenants/{tenantId}/datasync/connections/{connectionId}/edfi/educationorganizationidentificationsystemdescriptors | Retrieves a list of education organization identification system descriptors from an Ed-Fi API using the DataSync connection metadata
[**get_tenant_data_sync_connection_ed_fi_school_years**](ConnectionsEdFiApi.md#get_tenant_data_sync_connection_ed_fi_school_years) | **GET** /tenants/{tenantId}/datasync/connections/{connectionId}/edfi/schoolyears | Retrieves a list of school years from an Ed-Fi API using the DataSync connection metadata
[**get_tenant_data_sync_connection_ed_fi_staff_id_descriptors**](ConnectionsEdFiApi.md#get_tenant_data_sync_connection_ed_fi_staff_id_descriptors) | **GET** /tenants/{tenantId}/datasync/connections/{connectionId}/edfi/staffidentificationsystemdescriptors | Retrieves a list of staff identification system descriptors from an Ed-Fi API using the DataSync connection metadata
[**get_tenant_data_sync_connection_ed_fi_student_id_descriptors**](ConnectionsEdFiApi.md#get_tenant_data_sync_connection_ed_fi_student_id_descriptors) | **GET** /tenants/{tenantId}/datasync/connections/{connectionId}/edfi/studentidentificationsystemdescriptors | Retrieves a list of student identification system descriptors from an Ed-Fi API using the DataSync connection metadata
[**get_tenant_data_sync_connection_ed_fi_term_descriptors**](ConnectionsEdFiApi.md#get_tenant_data_sync_connection_ed_fi_term_descriptors) | **GET** /tenants/{tenantId}/datasync/connections/{connectionId}/edfi/termdescriptors | Retrieves a list of term descriptors from an Ed-Fi API using the DataSync connection metadata


# **get_tenant_data_sync_connection_ed_fi_districts**
> List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse] get_tenant_data_sync_connection_ed_fi_districts(tenant_id, connection_id)

Retrieves a list of districts from an Ed-Fi API using the DataSync connection metadata

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_connection_ed_fi_response import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse
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
    api_instance = edgraph_platform_client.ConnectionsEdFiApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    connection_id = 'connection_id_example' # str | 

    try:
        # Retrieves a list of districts from an Ed-Fi API using the DataSync connection metadata
        api_response = await api_instance.get_tenant_data_sync_connection_ed_fi_districts(tenant_id, connection_id)
        print("The response of ConnectionsEdFiApi->get_tenant_data_sync_connection_ed_fi_districts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsEdFiApi->get_tenant_data_sync_connection_ed_fi_districts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **connection_id** | **str**|  | 

### Return type

[**List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse]**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse.md)

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

# **get_tenant_data_sync_connection_ed_fi_education_organization_id_descriptors**
> List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse] get_tenant_data_sync_connection_ed_fi_education_organization_id_descriptors(tenant_id, connection_id)

Retrieves a list of education organization identification system descriptors from an Ed-Fi API using the DataSync connection metadata

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_connection_ed_fi_response import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse
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
    api_instance = edgraph_platform_client.ConnectionsEdFiApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    connection_id = 'connection_id_example' # str | 

    try:
        # Retrieves a list of education organization identification system descriptors from an Ed-Fi API using the DataSync connection metadata
        api_response = await api_instance.get_tenant_data_sync_connection_ed_fi_education_organization_id_descriptors(tenant_id, connection_id)
        print("The response of ConnectionsEdFiApi->get_tenant_data_sync_connection_ed_fi_education_organization_id_descriptors:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsEdFiApi->get_tenant_data_sync_connection_ed_fi_education_organization_id_descriptors: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **connection_id** | **str**|  | 

### Return type

[**List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse]**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse.md)

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

# **get_tenant_data_sync_connection_ed_fi_school_years**
> List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse] get_tenant_data_sync_connection_ed_fi_school_years(tenant_id, connection_id)

Retrieves a list of school years from an Ed-Fi API using the DataSync connection metadata

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_connection_ed_fi_response import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse
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
    api_instance = edgraph_platform_client.ConnectionsEdFiApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    connection_id = 'connection_id_example' # str | 

    try:
        # Retrieves a list of school years from an Ed-Fi API using the DataSync connection metadata
        api_response = await api_instance.get_tenant_data_sync_connection_ed_fi_school_years(tenant_id, connection_id)
        print("The response of ConnectionsEdFiApi->get_tenant_data_sync_connection_ed_fi_school_years:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsEdFiApi->get_tenant_data_sync_connection_ed_fi_school_years: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **connection_id** | **str**|  | 

### Return type

[**List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse]**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse.md)

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

# **get_tenant_data_sync_connection_ed_fi_staff_id_descriptors**
> List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse] get_tenant_data_sync_connection_ed_fi_staff_id_descriptors(tenant_id, connection_id)

Retrieves a list of staff identification system descriptors from an Ed-Fi API using the DataSync connection metadata

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_connection_ed_fi_response import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse
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
    api_instance = edgraph_platform_client.ConnectionsEdFiApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    connection_id = 'connection_id_example' # str | 

    try:
        # Retrieves a list of staff identification system descriptors from an Ed-Fi API using the DataSync connection metadata
        api_response = await api_instance.get_tenant_data_sync_connection_ed_fi_staff_id_descriptors(tenant_id, connection_id)
        print("The response of ConnectionsEdFiApi->get_tenant_data_sync_connection_ed_fi_staff_id_descriptors:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsEdFiApi->get_tenant_data_sync_connection_ed_fi_staff_id_descriptors: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **connection_id** | **str**|  | 

### Return type

[**List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse]**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse.md)

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

# **get_tenant_data_sync_connection_ed_fi_student_id_descriptors**
> List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse] get_tenant_data_sync_connection_ed_fi_student_id_descriptors(tenant_id, connection_id)

Retrieves a list of student identification system descriptors from an Ed-Fi API using the DataSync connection metadata

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_connection_ed_fi_response import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse
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
    api_instance = edgraph_platform_client.ConnectionsEdFiApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    connection_id = 'connection_id_example' # str | 

    try:
        # Retrieves a list of student identification system descriptors from an Ed-Fi API using the DataSync connection metadata
        api_response = await api_instance.get_tenant_data_sync_connection_ed_fi_student_id_descriptors(tenant_id, connection_id)
        print("The response of ConnectionsEdFiApi->get_tenant_data_sync_connection_ed_fi_student_id_descriptors:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsEdFiApi->get_tenant_data_sync_connection_ed_fi_student_id_descriptors: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **connection_id** | **str**|  | 

### Return type

[**List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse]**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse.md)

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

# **get_tenant_data_sync_connection_ed_fi_term_descriptors**
> List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse] get_tenant_data_sync_connection_ed_fi_term_descriptors(tenant_id, connection_id)

Retrieves a list of term descriptors from an Ed-Fi API using the DataSync connection metadata

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_connection_ed_fi_response import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse
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
    api_instance = edgraph_platform_client.ConnectionsEdFiApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    connection_id = 'connection_id_example' # str | 

    try:
        # Retrieves a list of term descriptors from an Ed-Fi API using the DataSync connection metadata
        api_response = await api_instance.get_tenant_data_sync_connection_ed_fi_term_descriptors(tenant_id, connection_id)
        print("The response of ConnectionsEdFiApi->get_tenant_data_sync_connection_ed_fi_term_descriptors:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsEdFiApi->get_tenant_data_sync_connection_ed_fi_term_descriptors: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **connection_id** | **str**|  | 

### Return type

[**List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse]**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesConnectionEdFiResponse.md)

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

