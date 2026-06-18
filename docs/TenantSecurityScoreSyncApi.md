# edgraph_platform_client.TenantSecurityScoreSyncApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_security_score_sync_job**](TenantSecurityScoreSyncApi.md#create_security_score_sync_job) | **POST** /tenants/{tenantId}/jobs/securityscore | Creates an Security Score Sync Job for a given tenant
[**execute_security_score_sync_job**](TenantSecurityScoreSyncApi.md#execute_security_score_sync_job) | **POST** /tenants/{tenantId}/jobs/securityscore/execute | Executes an Security Score Sync Job
[**get_security_score_sync_job**](TenantSecurityScoreSyncApi.md#get_security_score_sync_job) | **GET** /tenants/{tenantId}/jobs/securityscore | Retrieves a Security Score Sync Job for a given tenant
[**get_security_score_sync_job_execution**](TenantSecurityScoreSyncApi.md#get_security_score_sync_job_execution) | **GET** /tenants/{tenantId}/jobs/securityscore/{jobId}/executions/{jobExecutionId} | Retrieves a Security Score Sync Job Execution for a given tenant
[**update_security_score_sync_job**](TenantSecurityScoreSyncApi.md#update_security_score_sync_job) | **PUT** /tenants/{tenantId}/jobs/securityscore | Updates a Security Score Sync for a given tenant


# **create_security_score_sync_job**
> EdGraphHttpAggregatorsTenantApiServicesSecurityScoreSyncJobCreatedResult create_security_score_sync_job(tenant_id, ed_graph_http_aggregators_tenant_api_services_security_score_sync_create_security_score_sync_job_request=ed_graph_http_aggregators_tenant_api_services_security_score_sync_create_security_score_sync_job_request)

Creates an Security Score Sync Job for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_security_score_sync_create_security_score_sync_job_request import EdGraphHttpAggregatorsTenantApiServicesSecurityScoreSyncCreateSecurityScoreSyncJobRequest
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_security_score_sync_job_created_result import EdGraphHttpAggregatorsTenantApiServicesSecurityScoreSyncJobCreatedResult
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
    api_instance = edgraph_platform_client.TenantSecurityScoreSyncApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_services_security_score_sync_create_security_score_sync_job_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesSecurityScoreSyncCreateSecurityScoreSyncJobRequest() # EdGraphHttpAggregatorsTenantApiServicesSecurityScoreSyncCreateSecurityScoreSyncJobRequest |  (optional)

    try:
        # Creates an Security Score Sync Job for a given tenant
        api_response = await api_instance.create_security_score_sync_job(tenant_id, ed_graph_http_aggregators_tenant_api_services_security_score_sync_create_security_score_sync_job_request=ed_graph_http_aggregators_tenant_api_services_security_score_sync_create_security_score_sync_job_request)
        print("The response of TenantSecurityScoreSyncApi->create_security_score_sync_job:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantSecurityScoreSyncApi->create_security_score_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_services_security_score_sync_create_security_score_sync_job_request** | [**EdGraphHttpAggregatorsTenantApiServicesSecurityScoreSyncCreateSecurityScoreSyncJobRequest**](EdGraphHttpAggregatorsTenantApiServicesSecurityScoreSyncCreateSecurityScoreSyncJobRequest.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesSecurityScoreSyncJobCreatedResult**](EdGraphHttpAggregatorsTenantApiServicesSecurityScoreSyncJobCreatedResult.md)

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

# **execute_security_score_sync_job**
> execute_security_score_sync_job(tenant_id)

Executes an Security Score Sync Job

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
    api_instance = edgraph_platform_client.TenantSecurityScoreSyncApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Executes an Security Score Sync Job
        await api_instance.execute_security_score_sync_job(tenant_id)
    except Exception as e:
        print("Exception when calling TenantSecurityScoreSyncApi->execute_security_score_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 

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
**202** | Accepted |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**200** | The requested resource was successfully retrieved. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_security_score_sync_job**
> DataSyncApiSecurityScoreSyncV1SecurityScoreSyncProfile get_security_score_sync_job(tenant_id)

Retrieves a Security Score Sync Job for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_security_score_sync_v1_security_score_sync_profile import DataSyncApiSecurityScoreSyncV1SecurityScoreSyncProfile
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
    api_instance = edgraph_platform_client.TenantSecurityScoreSyncApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Retrieves a Security Score Sync Job for a given tenant
        api_response = await api_instance.get_security_score_sync_job(tenant_id)
        print("The response of TenantSecurityScoreSyncApi->get_security_score_sync_job:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantSecurityScoreSyncApi->get_security_score_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 

### Return type

[**DataSyncApiSecurityScoreSyncV1SecurityScoreSyncProfile**](DataSyncApiSecurityScoreSyncV1SecurityScoreSyncProfile.md)

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

# **get_security_score_sync_job_execution**
> DataSyncApiSecurityScoreSyncV1SecurityScoreSyncExecutionProfile get_security_score_sync_job_execution(tenant_id, job_id, job_execution_id)

Retrieves a Security Score Sync Job Execution for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_security_score_sync_v1_security_score_sync_execution_profile import DataSyncApiSecurityScoreSyncV1SecurityScoreSyncExecutionProfile
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
    api_instance = edgraph_platform_client.TenantSecurityScoreSyncApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    job_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    job_execution_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Retrieves a Security Score Sync Job Execution for a given tenant
        api_response = await api_instance.get_security_score_sync_job_execution(tenant_id, job_id, job_execution_id)
        print("The response of TenantSecurityScoreSyncApi->get_security_score_sync_job_execution:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantSecurityScoreSyncApi->get_security_score_sync_job_execution: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **job_id** | **UUID**|  | 
 **job_execution_id** | **UUID**|  | 

### Return type

[**DataSyncApiSecurityScoreSyncV1SecurityScoreSyncExecutionProfile**](DataSyncApiSecurityScoreSyncV1SecurityScoreSyncExecutionProfile.md)

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

# **update_security_score_sync_job**
> update_security_score_sync_job(tenant_id, ed_graph_http_aggregators_tenant_api_services_security_score_sync_update_security_score_sync_job_request=ed_graph_http_aggregators_tenant_api_services_security_score_sync_update_security_score_sync_job_request)

Updates a Security Score Sync for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_security_score_sync_update_security_score_sync_job_request import EdGraphHttpAggregatorsTenantApiServicesSecurityScoreSyncUpdateSecurityScoreSyncJobRequest
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
    api_instance = edgraph_platform_client.TenantSecurityScoreSyncApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_services_security_score_sync_update_security_score_sync_job_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesSecurityScoreSyncUpdateSecurityScoreSyncJobRequest() # EdGraphHttpAggregatorsTenantApiServicesSecurityScoreSyncUpdateSecurityScoreSyncJobRequest |  (optional)

    try:
        # Updates a Security Score Sync for a given tenant
        await api_instance.update_security_score_sync_job(tenant_id, ed_graph_http_aggregators_tenant_api_services_security_score_sync_update_security_score_sync_job_request=ed_graph_http_aggregators_tenant_api_services_security_score_sync_update_security_score_sync_job_request)
    except Exception as e:
        print("Exception when calling TenantSecurityScoreSyncApi->update_security_score_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **ed_graph_http_aggregators_tenant_api_services_security_score_sync_update_security_score_sync_job_request** | [**EdGraphHttpAggregatorsTenantApiServicesSecurityScoreSyncUpdateSecurityScoreSyncJobRequest**](EdGraphHttpAggregatorsTenantApiServicesSecurityScoreSyncUpdateSecurityScoreSyncJobRequest.md)|  | [optional] 

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
**204** | No Content |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**200** | The requested resource was successfully retrieved. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

