# edgraph_platform_client.CapacitiesApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**assign_my_group_to_capacity**](CapacitiesApi.md#assign_my_group_to_capacity) | **POST** /tenants/{tenantId}/analytics/capacities | Assigns the specified group to the specified capacity.
[**get_all_analytics_power_bi_capacities**](CapacitiesApi.md#get_all_analytics_power_bi_capacities) | **GET** /tenants/{tenantId}/analytics/capacities | Retrieves a list of capacities in Power Bi that the user has access to.
[**resume_capacity_async**](CapacitiesApi.md#resume_capacity_async) | **POST** /tenants/{tenantId}/analytics/capacities/resume | Resumes currently suspended capacity
[**suspend_capacity_async**](CapacitiesApi.md#suspend_capacity_async) | **POST** /tenants/{tenantId}/analytics/capacities/suspend | Suspends currently active capacity


# **assign_my_group_to_capacity**
> assign_my_group_to_capacity(tenant_id, analytics_api_capacities_v1_assign_capacity_request=analytics_api_capacities_v1_assign_capacity_request)

Assigns the specified group to the specified capacity.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_capacities_v1_assign_capacity_request import AnalyticsApiCapacitiesV1AssignCapacityRequest
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
    api_instance = edgraph_platform_client.CapacitiesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    analytics_api_capacities_v1_assign_capacity_request = edgraph_platform_client.AnalyticsApiCapacitiesV1AssignCapacityRequest() # AnalyticsApiCapacitiesV1AssignCapacityRequest |  (optional)

    try:
        # Assigns the specified group to the specified capacity.
        api_instance.assign_my_group_to_capacity(tenant_id, analytics_api_capacities_v1_assign_capacity_request=analytics_api_capacities_v1_assign_capacity_request)
    except Exception as e:
        print("Exception when calling CapacitiesApi->assign_my_group_to_capacity: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **analytics_api_capacities_v1_assign_capacity_request** | [**AnalyticsApiCapacitiesV1AssignCapacityRequest**](AnalyticsApiCapacitiesV1AssignCapacityRequest.md)|  | [optional] 

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
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_all_analytics_power_bi_capacities**
> AnalyticsApiCapacitiesV1CapacityResponse get_all_analytics_power_bi_capacities(tenant_id)

Retrieves a list of capacities in Power Bi that the user has access to.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_capacities_v1_capacity_response import AnalyticsApiCapacitiesV1CapacityResponse
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
    api_instance = edgraph_platform_client.CapacitiesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 

    try:
        # Retrieves a list of capacities in Power Bi that the user has access to.
        api_response = api_instance.get_all_analytics_power_bi_capacities(tenant_id)
        print("The response of CapacitiesApi->get_all_analytics_power_bi_capacities:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CapacitiesApi->get_all_analytics_power_bi_capacities: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 

### Return type

[**AnalyticsApiCapacitiesV1CapacityResponse**](AnalyticsApiCapacitiesV1CapacityResponse.md)

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

# **resume_capacity_async**
> resume_capacity_async(tenant_id, analytics_api_capacities_v1_resume_capacity_request=analytics_api_capacities_v1_resume_capacity_request)

Resumes currently suspended capacity

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_capacities_v1_resume_capacity_request import AnalyticsApiCapacitiesV1ResumeCapacityRequest
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
    api_instance = edgraph_platform_client.CapacitiesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    analytics_api_capacities_v1_resume_capacity_request = edgraph_platform_client.AnalyticsApiCapacitiesV1ResumeCapacityRequest() # AnalyticsApiCapacitiesV1ResumeCapacityRequest |  (optional)

    try:
        # Resumes currently suspended capacity
        api_instance.resume_capacity_async(tenant_id, analytics_api_capacities_v1_resume_capacity_request=analytics_api_capacities_v1_resume_capacity_request)
    except Exception as e:
        print("Exception when calling CapacitiesApi->resume_capacity_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **analytics_api_capacities_v1_resume_capacity_request** | [**AnalyticsApiCapacitiesV1ResumeCapacityRequest**](AnalyticsApiCapacitiesV1ResumeCapacityRequest.md)|  | [optional] 

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
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **suspend_capacity_async**
> suspend_capacity_async(tenant_id, analytics_api_capacities_v1_suspend_capacity_request=analytics_api_capacities_v1_suspend_capacity_request)

Suspends currently active capacity

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_capacities_v1_suspend_capacity_request import AnalyticsApiCapacitiesV1SuspendCapacityRequest
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
    api_instance = edgraph_platform_client.CapacitiesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    analytics_api_capacities_v1_suspend_capacity_request = edgraph_platform_client.AnalyticsApiCapacitiesV1SuspendCapacityRequest() # AnalyticsApiCapacitiesV1SuspendCapacityRequest |  (optional)

    try:
        # Suspends currently active capacity
        api_instance.suspend_capacity_async(tenant_id, analytics_api_capacities_v1_suspend_capacity_request=analytics_api_capacities_v1_suspend_capacity_request)
    except Exception as e:
        print("Exception when calling CapacitiesApi->suspend_capacity_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **analytics_api_capacities_v1_suspend_capacity_request** | [**AnalyticsApiCapacitiesV1SuspendCapacityRequest**](AnalyticsApiCapacitiesV1SuspendCapacityRequest.md)|  | [optional] 

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
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

