# edgraph_platform_client.TenantJobsInstructionalInsightsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_instructional_insights_security_sync_job**](TenantJobsInstructionalInsightsApi.md#create_instructional_insights_security_sync_job) | **POST** /tenants/{tenantId}/jobs/instructionalinsights | Creates an Instructional Insights Security Sync Job for a given tenant
[**execute_instructional_insights_security_sync_job**](TenantJobsInstructionalInsightsApi.md#execute_instructional_insights_security_sync_job) | **POST** /tenants/{tenantId}/jobs/instructionalinsights/execute | Executes an Instructional Insights Security Sync Job
[**get_instructional_insights_security_sync_job**](TenantJobsInstructionalInsightsApi.md#get_instructional_insights_security_sync_job) | **GET** /tenants/{tenantId}/jobs/instructionalinsights | Retrieves an Instructional Insights Security Sync Job for a given tenant
[**search_instructional_insights_security_sync_job_execution_logs**](TenantJobsInstructionalInsightsApi.md#search_instructional_insights_security_sync_job_execution_logs) | **GET** /tenants/{tenantId}/jobs/instructionalinsights/executions/{executionId}/logs | Searches Instructional Insights Security Sync Job Execution Logs for a given tenant and execution
[**search_instructional_insights_security_sync_job_executions**](TenantJobsInstructionalInsightsApi.md#search_instructional_insights_security_sync_job_executions) | **GET** /tenants/{tenantId}/jobs/instructionalinsights/executions | Searches Instructional Insights Security Sync Job Executions for a given tenant
[**update_instructional_insights_security_sync_job**](TenantJobsInstructionalInsightsApi.md#update_instructional_insights_security_sync_job) | **PUT** /tenants/{tenantId}/jobs/instructionalinsights | Updates an Instructional Insights Security Sync Job for a given tenant


# **create_instructional_insights_security_sync_job**
> IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobCreatedResponse create_instructional_insights_security_sync_job(tenant_id, identity_api_instructional_insights_v1_create_instructional_insights_security_sync_job_request=identity_api_instructional_insights_v1_create_instructional_insights_security_sync_job_request)

Creates an Instructional Insights Security Sync Job for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_instructional_insights_v1_create_instructional_insights_security_sync_job_request import IdentityApiInstructionalInsightsV1CreateInstructionalInsightsSecuritySyncJobRequest
from edgraph_platform_client.models.identity_api_instructional_insights_v1_instructional_insights_security_sync_job_created_response import IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobCreatedResponse
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
    api_instance = edgraph_platform_client.TenantJobsInstructionalInsightsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    identity_api_instructional_insights_v1_create_instructional_insights_security_sync_job_request = edgraph_platform_client.IdentityApiInstructionalInsightsV1CreateInstructionalInsightsSecuritySyncJobRequest() # IdentityApiInstructionalInsightsV1CreateInstructionalInsightsSecuritySyncJobRequest |  (optional)

    try:
        # Creates an Instructional Insights Security Sync Job for a given tenant
        api_response = await api_instance.create_instructional_insights_security_sync_job(tenant_id, identity_api_instructional_insights_v1_create_instructional_insights_security_sync_job_request=identity_api_instructional_insights_v1_create_instructional_insights_security_sync_job_request)
        print("The response of TenantJobsInstructionalInsightsApi->create_instructional_insights_security_sync_job:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantJobsInstructionalInsightsApi->create_instructional_insights_security_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **identity_api_instructional_insights_v1_create_instructional_insights_security_sync_job_request** | [**IdentityApiInstructionalInsightsV1CreateInstructionalInsightsSecuritySyncJobRequest**](IdentityApiInstructionalInsightsV1CreateInstructionalInsightsSecuritySyncJobRequest.md)|  | [optional] 

### Return type

[**IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobCreatedResponse**](IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobCreatedResponse.md)

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

# **execute_instructional_insights_security_sync_job**
> IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutedResponse execute_instructional_insights_security_sync_job(tenant_id)

Executes an Instructional Insights Security Sync Job

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_instructional_insights_v1_instructional_insights_security_sync_job_executed_response import IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutedResponse
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
    api_instance = edgraph_platform_client.TenantJobsInstructionalInsightsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Executes an Instructional Insights Security Sync Job
        api_response = await api_instance.execute_instructional_insights_security_sync_job(tenant_id)
        print("The response of TenantJobsInstructionalInsightsApi->execute_instructional_insights_security_sync_job:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantJobsInstructionalInsightsApi->execute_instructional_insights_security_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 

### Return type

[**IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutedResponse**](IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutedResponse.md)

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
**202** | The job execution was successfully requested. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_instructional_insights_security_sync_job**
> IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobResponse get_instructional_insights_security_sync_job(tenant_id)

Retrieves an Instructional Insights Security Sync Job for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_instructional_insights_v1_instructional_insights_security_sync_job_response import IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobResponse
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
    api_instance = edgraph_platform_client.TenantJobsInstructionalInsightsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Retrieves an Instructional Insights Security Sync Job for a given tenant
        api_response = await api_instance.get_instructional_insights_security_sync_job(tenant_id)
        print("The response of TenantJobsInstructionalInsightsApi->get_instructional_insights_security_sync_job:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantJobsInstructionalInsightsApi->get_instructional_insights_security_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 

### Return type

[**IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobResponse**](IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobResponse.md)

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

# **search_instructional_insights_security_sync_job_execution_logs**
> IdentityApiInstructionalInsightsV1SearchInstructionalInsightsSecuritySyncJobExecutionLogsResponse search_instructional_insights_security_sync_job_execution_logs(tenant_id, execution_id, job_id=job_id, page_index=page_index, page_size=page_size, order_by=order_by, level=level, message=message)

Searches Instructional Insights Security Sync Job Execution Logs for a given tenant and execution

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_instructional_insights_v1_search_instructional_insights_security_sync_job_execution_logs_response import IdentityApiInstructionalInsightsV1SearchInstructionalInsightsSecuritySyncJobExecutionLogsResponse
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
    api_instance = edgraph_platform_client.TenantJobsInstructionalInsightsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    execution_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    job_id = '' # str |  (optional) (default to '')
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = '' # str |  (optional) (default to '')
    level = '' # str |  (optional) (default to '')
    message = '' # str |  (optional) (default to '')

    try:
        # Searches Instructional Insights Security Sync Job Execution Logs for a given tenant and execution
        api_response = await api_instance.search_instructional_insights_security_sync_job_execution_logs(tenant_id, execution_id, job_id=job_id, page_index=page_index, page_size=page_size, order_by=order_by, level=level, message=message)
        print("The response of TenantJobsInstructionalInsightsApi->search_instructional_insights_security_sync_job_execution_logs:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantJobsInstructionalInsightsApi->search_instructional_insights_security_sync_job_execution_logs: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **execution_id** | **UUID**|  | 
 **job_id** | **str**|  | [optional] [default to &#39;&#39;]
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **level** | **str**|  | [optional] [default to &#39;&#39;]
 **message** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**IdentityApiInstructionalInsightsV1SearchInstructionalInsightsSecuritySyncJobExecutionLogsResponse**](IdentityApiInstructionalInsightsV1SearchInstructionalInsightsSecuritySyncJobExecutionLogsResponse.md)

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

# **search_instructional_insights_security_sync_job_executions**
> IdentityApiInstructionalInsightsV1SearchInstructionalInsightsSecuritySyncJobExecutionsResponse search_instructional_insights_security_sync_job_executions(tenant_id, job_id=job_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)

Searches Instructional Insights Security Sync Job Executions for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_instructional_insights_v1_search_instructional_insights_security_sync_job_executions_response import IdentityApiInstructionalInsightsV1SearchInstructionalInsightsSecuritySyncJobExecutionsResponse
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
    api_instance = edgraph_platform_client.TenantJobsInstructionalInsightsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    job_id = '' # str |  (optional) (default to '')
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Searches Instructional Insights Security Sync Job Executions for a given tenant
        api_response = await api_instance.search_instructional_insights_security_sync_job_executions(tenant_id, job_id=job_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)
        print("The response of TenantJobsInstructionalInsightsApi->search_instructional_insights_security_sync_job_executions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantJobsInstructionalInsightsApi->search_instructional_insights_security_sync_job_executions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **job_id** | **str**|  | [optional] [default to &#39;&#39;]
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**IdentityApiInstructionalInsightsV1SearchInstructionalInsightsSecuritySyncJobExecutionsResponse**](IdentityApiInstructionalInsightsV1SearchInstructionalInsightsSecuritySyncJobExecutionsResponse.md)

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

# **update_instructional_insights_security_sync_job**
> MicrosoftAspNetCoreMvcNoContentResult update_instructional_insights_security_sync_job(tenant_id, identity_api_instructional_insights_v1_update_instructional_insights_security_sync_job_request=identity_api_instructional_insights_v1_update_instructional_insights_security_sync_job_request)

Updates an Instructional Insights Security Sync Job for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_instructional_insights_v1_update_instructional_insights_security_sync_job_request import IdentityApiInstructionalInsightsV1UpdateInstructionalInsightsSecuritySyncJobRequest
from edgraph_platform_client.models.microsoft_asp_net_core_mvc_no_content_result import MicrosoftAspNetCoreMvcNoContentResult
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
    api_instance = edgraph_platform_client.TenantJobsInstructionalInsightsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    identity_api_instructional_insights_v1_update_instructional_insights_security_sync_job_request = edgraph_platform_client.IdentityApiInstructionalInsightsV1UpdateInstructionalInsightsSecuritySyncJobRequest() # IdentityApiInstructionalInsightsV1UpdateInstructionalInsightsSecuritySyncJobRequest |  (optional)

    try:
        # Updates an Instructional Insights Security Sync Job for a given tenant
        api_response = await api_instance.update_instructional_insights_security_sync_job(tenant_id, identity_api_instructional_insights_v1_update_instructional_insights_security_sync_job_request=identity_api_instructional_insights_v1_update_instructional_insights_security_sync_job_request)
        print("The response of TenantJobsInstructionalInsightsApi->update_instructional_insights_security_sync_job:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantJobsInstructionalInsightsApi->update_instructional_insights_security_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **identity_api_instructional_insights_v1_update_instructional_insights_security_sync_job_request** | [**IdentityApiInstructionalInsightsV1UpdateInstructionalInsightsSecuritySyncJobRequest**](IdentityApiInstructionalInsightsV1UpdateInstructionalInsightsSecuritySyncJobRequest.md)|  | [optional] 

### Return type

[**MicrosoftAspNetCoreMvcNoContentResult**](MicrosoftAspNetCoreMvcNoContentResult.md)

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
**204** | The resource was successfully updated. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

