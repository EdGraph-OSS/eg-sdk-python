# edgraph_platform_client.TenantJobsDSLApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_dsl_job**](TenantJobsDSLApi.md#create_dsl_job) | **POST** /tenants/{tenantId}/jobs/dsl | Creates a DSL Sync Job for a given tenant
[**execute_dsl_job**](TenantJobsDSLApi.md#execute_dsl_job) | **PUT** /tenants/{tenantId}/jobs/dsl/{jobId}/execute | Executes a DSL Sync Job for a given tenant
[**get_dsl_job**](TenantJobsDSLApi.md#get_dsl_job) | **GET** /tenants/{tenantId}/jobs/dsl/{jobId} | Retrieves a DSL jobs profile for a given tenant
[**update_dsl_job**](TenantJobsDSLApi.md#update_dsl_job) | **PUT** /tenants/{tenantId}/jobs/dsl/{jobId} | Updates a DSL Sync Job for a given tenant


# **create_dsl_job**
> DataSyncApiDslV1JobCreatedResponse create_dsl_job(tenant_id, data_sync_api_dsl_v1_create_job_request=data_sync_api_dsl_v1_create_job_request)

Creates a DSL Sync Job for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_dsl_v1_create_job_request import DataSyncApiDslV1CreateJobRequest
from edgraph_platform_client.models.data_sync_api_dsl_v1_job_created_response import DataSyncApiDslV1JobCreatedResponse
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
    api_instance = edgraph_platform_client.TenantJobsDSLApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    data_sync_api_dsl_v1_create_job_request = edgraph_platform_client.DataSyncApiDslV1CreateJobRequest() # DataSyncApiDslV1CreateJobRequest |  (optional)

    try:
        # Creates a DSL Sync Job for a given tenant
        api_response = await api_instance.create_dsl_job(tenant_id, data_sync_api_dsl_v1_create_job_request=data_sync_api_dsl_v1_create_job_request)
        print("The response of TenantJobsDSLApi->create_dsl_job:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantJobsDSLApi->create_dsl_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **data_sync_api_dsl_v1_create_job_request** | [**DataSyncApiDslV1CreateJobRequest**](DataSyncApiDslV1CreateJobRequest.md)|  | [optional] 

### Return type

[**DataSyncApiDslV1JobCreatedResponse**](DataSyncApiDslV1JobCreatedResponse.md)

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

# **execute_dsl_job**
> DataSyncApiDslV1DslJobExecutedResponse execute_dsl_job(tenant_id, job_id)

Executes a DSL Sync Job for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_dsl_v1_dsl_job_executed_response import DataSyncApiDslV1DslJobExecutedResponse
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
    api_instance = edgraph_platform_client.TenantJobsDSLApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    job_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Executes a DSL Sync Job for a given tenant
        api_response = await api_instance.execute_dsl_job(tenant_id, job_id)
        print("The response of TenantJobsDSLApi->execute_dsl_job:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantJobsDSLApi->execute_dsl_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **job_id** | **UUID**|  | 

### Return type

[**DataSyncApiDslV1DslJobExecutedResponse**](DataSyncApiDslV1DslJobExecutedResponse.md)

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

# **get_dsl_job**
> DataSyncApiDslV1DslProfile get_dsl_job(tenant_id, job_id)

Retrieves a DSL jobs profile for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_dsl_v1_dsl_profile import DataSyncApiDslV1DslProfile
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
    api_instance = edgraph_platform_client.TenantJobsDSLApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    job_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Retrieves a DSL jobs profile for a given tenant
        api_response = await api_instance.get_dsl_job(tenant_id, job_id)
        print("The response of TenantJobsDSLApi->get_dsl_job:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantJobsDSLApi->get_dsl_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **job_id** | **UUID**|  | 

### Return type

[**DataSyncApiDslV1DslProfile**](DataSyncApiDslV1DslProfile.md)

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

# **update_dsl_job**
> object update_dsl_job(tenant_id, job_id, data_sync_api_dsl_v1_update_job_request=data_sync_api_dsl_v1_update_job_request)

Updates a DSL Sync Job for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_dsl_v1_update_job_request import DataSyncApiDslV1UpdateJobRequest
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
    api_instance = edgraph_platform_client.TenantJobsDSLApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    job_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    data_sync_api_dsl_v1_update_job_request = edgraph_platform_client.DataSyncApiDslV1UpdateJobRequest() # DataSyncApiDslV1UpdateJobRequest |  (optional)

    try:
        # Updates a DSL Sync Job for a given tenant
        api_response = await api_instance.update_dsl_job(tenant_id, job_id, data_sync_api_dsl_v1_update_job_request=data_sync_api_dsl_v1_update_job_request)
        print("The response of TenantJobsDSLApi->update_dsl_job:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantJobsDSLApi->update_dsl_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **job_id** | **UUID**|  | 
 **data_sync_api_dsl_v1_update_job_request** | [**DataSyncApiDslV1UpdateJobRequest**](DataSyncApiDslV1UpdateJobRequest.md)|  | [optional] 

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
**200** | Success |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**204** | The resource was successfully updated. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

