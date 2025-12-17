# edgraph_platform_client.EnvironmentsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_environment**](EnvironmentsApi.md#create_environment) | **POST** /tenants/{tenantId}/validations/environments | Creates an Environment.
[**create_state_reporting_environment**](EnvironmentsApi.md#create_state_reporting_environment) | **POST** /tenants/{tenantId}/statereporting/environments | Creates a new Environment.
[**delete_environment**](EnvironmentsApi.md#delete_environment) | **DELETE** /tenants/{tenantId}/validations/environments/{environmentId} | Deletes an Environment.
[**delete_state_reporting_environment**](EnvironmentsApi.md#delete_state_reporting_environment) | **DELETE** /tenants/{tenantId}/statereporting/environments/{environmentId} | Deletes an Environment.
[**get_environment_by_id**](EnvironmentsApi.md#get_environment_by_id) | **GET** /tenants/{tenantId}/validations/environments/{environmentId} | Retrieves an Environment by ID.
[**get_environments**](EnvironmentsApi.md#get_environments) | **GET** /tenants/{tenantId}/validations/environments | Retrieves a list of Environments.
[**get_state_reporting_environment**](EnvironmentsApi.md#get_state_reporting_environment) | **GET** /tenants/{tenantId}/statereporting/environments/{environmentId} | Retrieves an Environment by ID.
[**search_state_reporting_environments**](EnvironmentsApi.md#search_state_reporting_environments) | **GET** /tenants/{tenantId}/statereporting/environments | Retrieves a list of Environments.
[**test_environment_connection**](EnvironmentsApi.md#test_environment_connection) | **POST** /tenants/{tenantId}/validations/environments/testconnection | Tests if the provided connection string can establish a valid connection.
[**update_environment**](EnvironmentsApi.md#update_environment) | **PUT** /tenants/{tenantId}/validations/environments/{environmentId} | Updates an Environment.
[**update_state_reporting_environment**](EnvironmentsApi.md#update_state_reporting_environment) | **PUT** /tenants/{tenantId}/statereporting/environments/{environmentId} | Updates an Environment.


# **create_environment**
> ValidationsApiCoreV1CreatedResponse create_environment(tenant_id, validations_api_db_environments_v1_create_request=validations_api_db_environments_v1_create_request)

Creates an Environment.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_core_v1_created_response import ValidationsApiCoreV1CreatedResponse
from edgraph_platform_client.models.validations_api_db_environments_v1_create_request import ValidationsApiDbEnvironmentsV1CreateRequest
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
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.EnvironmentsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    validations_api_db_environments_v1_create_request = edgraph_platform_client.ValidationsApiDbEnvironmentsV1CreateRequest() # ValidationsApiDbEnvironmentsV1CreateRequest |  (optional)

    try:
        # Creates an Environment.
        api_response = api_instance.create_environment(tenant_id, validations_api_db_environments_v1_create_request=validations_api_db_environments_v1_create_request)
        print("The response of EnvironmentsApi->create_environment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsApi->create_environment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **validations_api_db_environments_v1_create_request** | [**ValidationsApiDbEnvironmentsV1CreateRequest**](ValidationsApiDbEnvironmentsV1CreateRequest.md)|  | [optional] 

### Return type

[**ValidationsApiCoreV1CreatedResponse**](ValidationsApiCoreV1CreatedResponse.md)

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

# **create_state_reporting_environment**
> EdGraphServicesStateReportingV1EnvironmentCreatedResponse create_state_reporting_environment(tenant_id, ed_graph_services_state_reporting_v1_create_environment_request=ed_graph_services_state_reporting_v1_create_environment_request)

Creates a new Environment.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_create_environment_request import EdGraphServicesStateReportingV1CreateEnvironmentRequest
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_environment_created_response import EdGraphServicesStateReportingV1EnvironmentCreatedResponse
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
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.EnvironmentsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_services_state_reporting_v1_create_environment_request = edgraph_platform_client.EdGraphServicesStateReportingV1CreateEnvironmentRequest() # EdGraphServicesStateReportingV1CreateEnvironmentRequest |  (optional)

    try:
        # Creates a new Environment.
        api_response = api_instance.create_state_reporting_environment(tenant_id, ed_graph_services_state_reporting_v1_create_environment_request=ed_graph_services_state_reporting_v1_create_environment_request)
        print("The response of EnvironmentsApi->create_state_reporting_environment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsApi->create_state_reporting_environment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_services_state_reporting_v1_create_environment_request** | [**EdGraphServicesStateReportingV1CreateEnvironmentRequest**](EdGraphServicesStateReportingV1CreateEnvironmentRequest.md)|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1EnvironmentCreatedResponse**](EdGraphServicesStateReportingV1EnvironmentCreatedResponse.md)

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

# **delete_environment**
> delete_environment(tenant_id, environment_id)

Deletes an Environment.

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
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.EnvironmentsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 

    try:
        # Deletes an Environment.
        api_instance.delete_environment(tenant_id, environment_id)
    except Exception as e:
        print("Exception when calling EnvironmentsApi->delete_environment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 

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

# **delete_state_reporting_environment**
> EdGraphServicesStateReportingV1EnvironmentDeletedResponse delete_state_reporting_environment(tenant_id, environment_id)

Deletes an Environment.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_environment_deleted_response import EdGraphServicesStateReportingV1EnvironmentDeletedResponse
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
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.EnvironmentsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 

    try:
        # Deletes an Environment.
        api_response = api_instance.delete_state_reporting_environment(tenant_id, environment_id)
        print("The response of EnvironmentsApi->delete_state_reporting_environment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsApi->delete_state_reporting_environment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 

### Return type

[**EdGraphServicesStateReportingV1EnvironmentDeletedResponse**](EdGraphServicesStateReportingV1EnvironmentDeletedResponse.md)

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

# **get_environment_by_id**
> ValidationsApiDbEnvironmentsV1DbEnvironmentDto get_environment_by_id(tenant_id, environment_id)

Retrieves an Environment by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_db_environments_v1_db_environment_dto import ValidationsApiDbEnvironmentsV1DbEnvironmentDto
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
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.EnvironmentsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 

    try:
        # Retrieves an Environment by ID.
        api_response = api_instance.get_environment_by_id(tenant_id, environment_id)
        print("The response of EnvironmentsApi->get_environment_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsApi->get_environment_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 

### Return type

[**ValidationsApiDbEnvironmentsV1DbEnvironmentDto**](ValidationsApiDbEnvironmentsV1DbEnvironmentDto.md)

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

# **get_environments**
> ValidationsApiDbEnvironmentsV1PaginatedDbEnvironments get_environments(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)

Retrieves a list of Environments.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_db_environments_v1_paginated_db_environments import ValidationsApiDbEnvironmentsV1PaginatedDbEnvironments
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
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.EnvironmentsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    filter = 'filter_example' # str |  (optional)
    order_by = 'order_by_example' # str |  (optional)

    try:
        # Retrieves a list of Environments.
        api_response = api_instance.get_environments(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)
        print("The response of EnvironmentsApi->get_environments:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsApi->get_environments: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **filter** | **str**|  | [optional] 
 **order_by** | **str**|  | [optional] 

### Return type

[**ValidationsApiDbEnvironmentsV1PaginatedDbEnvironments**](ValidationsApiDbEnvironmentsV1PaginatedDbEnvironments.md)

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

# **get_state_reporting_environment**
> EdGraphServicesStateReportingV1EnvironmentProfileResponse get_state_reporting_environment(tenant_id, environment_id)

Retrieves an Environment by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_environment_profile_response import EdGraphServicesStateReportingV1EnvironmentProfileResponse
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
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.EnvironmentsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 

    try:
        # Retrieves an Environment by ID.
        api_response = api_instance.get_state_reporting_environment(tenant_id, environment_id)
        print("The response of EnvironmentsApi->get_state_reporting_environment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsApi->get_state_reporting_environment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 

### Return type

[**EdGraphServicesStateReportingV1EnvironmentProfileResponse**](EdGraphServicesStateReportingV1EnvironmentProfileResponse.md)

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

# **search_state_reporting_environments**
> EdGraphServicesStateReportingV1PaginatedEnvironmentsResponse search_state_reporting_environments(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)

Retrieves a list of Environments.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_paginated_environments_response import EdGraphServicesStateReportingV1PaginatedEnvironmentsResponse
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
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.EnvironmentsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = 'order_by_example' # str |  (optional)
    filter = 'filter_example' # str |  (optional)

    try:
        # Retrieves a list of Environments.
        api_response = api_instance.search_state_reporting_environments(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)
        print("The response of EnvironmentsApi->search_state_reporting_environments:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsApi->search_state_reporting_environments: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **order_by** | **str**|  | [optional] 
 **filter** | **str**|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1PaginatedEnvironmentsResponse**](EdGraphServicesStateReportingV1PaginatedEnvironmentsResponse.md)

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

# **test_environment_connection**
> ValidationsApiDbEnvironmentsV1TestConnectionResponse test_environment_connection(tenant_id, validations_api_db_environments_v1_test_connection_request=validations_api_db_environments_v1_test_connection_request)

Tests if the provided connection string can establish a valid connection.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_db_environments_v1_test_connection_request import ValidationsApiDbEnvironmentsV1TestConnectionRequest
from edgraph_platform_client.models.validations_api_db_environments_v1_test_connection_response import ValidationsApiDbEnvironmentsV1TestConnectionResponse
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
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.EnvironmentsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    validations_api_db_environments_v1_test_connection_request = edgraph_platform_client.ValidationsApiDbEnvironmentsV1TestConnectionRequest() # ValidationsApiDbEnvironmentsV1TestConnectionRequest |  (optional)

    try:
        # Tests if the provided connection string can establish a valid connection.
        api_response = api_instance.test_environment_connection(tenant_id, validations_api_db_environments_v1_test_connection_request=validations_api_db_environments_v1_test_connection_request)
        print("The response of EnvironmentsApi->test_environment_connection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsApi->test_environment_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **validations_api_db_environments_v1_test_connection_request** | [**ValidationsApiDbEnvironmentsV1TestConnectionRequest**](ValidationsApiDbEnvironmentsV1TestConnectionRequest.md)|  | [optional] 

### Return type

[**ValidationsApiDbEnvironmentsV1TestConnectionResponse**](ValidationsApiDbEnvironmentsV1TestConnectionResponse.md)

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

# **update_environment**
> object update_environment(tenant_id, environment_id, validations_api_db_environments_v1_update_request=validations_api_db_environments_v1_update_request)

Updates an Environment.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_db_environments_v1_update_request import ValidationsApiDbEnvironmentsV1UpdateRequest
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
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.EnvironmentsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    validations_api_db_environments_v1_update_request = edgraph_platform_client.ValidationsApiDbEnvironmentsV1UpdateRequest() # ValidationsApiDbEnvironmentsV1UpdateRequest |  (optional)

    try:
        # Updates an Environment.
        api_response = api_instance.update_environment(tenant_id, environment_id, validations_api_db_environments_v1_update_request=validations_api_db_environments_v1_update_request)
        print("The response of EnvironmentsApi->update_environment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsApi->update_environment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **validations_api_db_environments_v1_update_request** | [**ValidationsApiDbEnvironmentsV1UpdateRequest**](ValidationsApiDbEnvironmentsV1UpdateRequest.md)|  | [optional] 

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
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_state_reporting_environment**
> EdGraphServicesStateReportingV1EnvironmentUpdatedResponse update_state_reporting_environment(tenant_id, environment_id, ed_graph_services_state_reporting_v1_update_environment_request=ed_graph_services_state_reporting_v1_update_environment_request)

Updates an Environment.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_environment_updated_response import EdGraphServicesStateReportingV1EnvironmentUpdatedResponse
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_update_environment_request import EdGraphServicesStateReportingV1UpdateEnvironmentRequest
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
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.EnvironmentsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    ed_graph_services_state_reporting_v1_update_environment_request = edgraph_platform_client.EdGraphServicesStateReportingV1UpdateEnvironmentRequest() # EdGraphServicesStateReportingV1UpdateEnvironmentRequest |  (optional)

    try:
        # Updates an Environment.
        api_response = api_instance.update_state_reporting_environment(tenant_id, environment_id, ed_graph_services_state_reporting_v1_update_environment_request=ed_graph_services_state_reporting_v1_update_environment_request)
        print("The response of EnvironmentsApi->update_state_reporting_environment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsApi->update_state_reporting_environment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **ed_graph_services_state_reporting_v1_update_environment_request** | [**EdGraphServicesStateReportingV1UpdateEnvironmentRequest**](EdGraphServicesStateReportingV1UpdateEnvironmentRequest.md)|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1EnvironmentUpdatedResponse**](EdGraphServicesStateReportingV1EnvironmentUpdatedResponse.md)

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

