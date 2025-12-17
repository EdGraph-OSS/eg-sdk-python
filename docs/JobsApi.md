# edgraph_platform_client.JobsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**activate_tenant_data_sync_job**](JobsApi.md#activate_tenant_data_sync_job) | **POST** /tenants/{tenantId}/datasync/jobs/{jobId}/activate | Activate a DataSync job matching the primary key
[**cancel_job**](JobsApi.md#cancel_job) | **POST** /tenants/{tenantId}/validations/jobs/{jobId}/cancel | Requests a Job cancellation.
[**cancel_tenant_data_sync_job**](JobsApi.md#cancel_tenant_data_sync_job) | **POST** /tenants/{tenantId}/datasync/jobs/{jobId}/cancel | Cancel a DataSync job matching the primary key
[**create_job**](JobsApi.md#create_job) | **POST** /tenants/{tenantId}/validations/jobs | Creates a Job.
[**create_tenant_data_sync_job**](JobsApi.md#create_tenant_data_sync_job) | **POST** /tenants/{tenantId}/datasync/jobs | Creates a new DataSync job
[**deactivate_tenant_data_sync_job**](JobsApi.md#deactivate_tenant_data_sync_job) | **POST** /tenants/{tenantId}/datasync/jobs/{jobId}/deactivate | Deactivate a DataSync job matching the primary key
[**delete_job**](JobsApi.md#delete_job) | **DELETE** /tenants/{tenantId}/validations/jobs/{jobId} | Deletes a Job.
[**delete_tenant_data_sync_job**](JobsApi.md#delete_tenant_data_sync_job) | **DELETE** /tenants/{tenantId}/datasync/jobs/{jobId} | Delete a DataSync job matching the primary key
[**execute_job**](JobsApi.md#execute_job) | **POST** /tenants/{tenantId}/validations/jobs/{jobId}/execute | Requests a Job execution.
[**execute_tenant_data_sync_job**](JobsApi.md#execute_tenant_data_sync_job) | **POST** /tenants/{tenantId}/datasync/jobs/{jobId}/execute | Execute a DataSync job matching the primary key
[**get_all_tenant_data_sync_jobs**](JobsApi.md#get_all_tenant_data_sync_jobs) | **GET** /tenants/{tenantId}/datasync/jobs | Retrieves a list of DataSync Jobs
[**get_job_by_id**](JobsApi.md#get_job_by_id) | **GET** /tenants/{tenantId}/validations/jobs/{jobId} | Retrieves a Job by ID.
[**get_jobs**](JobsApi.md#get_jobs) | **GET** /tenants/{tenantId}/validations/jobs | Retrieves a list of Jobs.
[**get_tenant_data_sync_job_profile_by_id**](JobsApi.md#get_tenant_data_sync_job_profile_by_id) | **GET** /tenants/{tenantId}/datasync/jobs/{jobId} | Retrieves a specific DataSync job using its primary key
[**restart_job_schedule**](JobsApi.md#restart_job_schedule) | **POST** /tenants/{tenantId}/validations/jobs/{jobId}/restart | Requests a Job schedule restart.
[**update_job**](JobsApi.md#update_job) | **PUT** /tenants/{tenantId}/validations/jobs/{jobId} | Updates a Job.
[**update_tenant_data_sync_job**](JobsApi.md#update_tenant_data_sync_job) | **PUT** /tenants/{tenantId}/datasync/jobs/{jobId} | Updates a DataSync job matching the primary key


# **activate_tenant_data_sync_job**
> activate_tenant_data_sync_job(tenant_id, job_id, data_sync_api_job_v1_activate_job_request=data_sync_api_job_v1_activate_job_request)

Activate a DataSync job matching the primary key

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_job_v1_activate_job_request import DataSyncApiJobV1ActivateJobRequest
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
    api_instance = edgraph_platform_client.JobsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 
    data_sync_api_job_v1_activate_job_request = edgraph_platform_client.DataSyncApiJobV1ActivateJobRequest() # DataSyncApiJobV1ActivateJobRequest |  (optional)

    try:
        # Activate a DataSync job matching the primary key
        api_instance.activate_tenant_data_sync_job(tenant_id, job_id, data_sync_api_job_v1_activate_job_request=data_sync_api_job_v1_activate_job_request)
    except Exception as e:
        print("Exception when calling JobsApi->activate_tenant_data_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 
 **data_sync_api_job_v1_activate_job_request** | [**DataSyncApiJobV1ActivateJobRequest**](DataSyncApiJobV1ActivateJobRequest.md)|  | [optional] 

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
**202** | The request has been accepted for processing, but the processing is not yet complete. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cancel_job**
> object cancel_job(tenant_id, job_id)

Requests a Job cancellation.

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
    api_instance = edgraph_platform_client.JobsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 

    try:
        # Requests a Job cancellation.
        api_response = api_instance.cancel_job(tenant_id, job_id)
        print("The response of JobsApi->cancel_job:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling JobsApi->cancel_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 

### Return type

**object**

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

# **cancel_tenant_data_sync_job**
> cancel_tenant_data_sync_job(tenant_id, job_id, data_sync_api_job_v1_cancel_job_request=data_sync_api_job_v1_cancel_job_request)

Cancel a DataSync job matching the primary key

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_job_v1_cancel_job_request import DataSyncApiJobV1CancelJobRequest
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
    api_instance = edgraph_platform_client.JobsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 
    data_sync_api_job_v1_cancel_job_request = edgraph_platform_client.DataSyncApiJobV1CancelJobRequest() # DataSyncApiJobV1CancelJobRequest |  (optional)

    try:
        # Cancel a DataSync job matching the primary key
        api_instance.cancel_tenant_data_sync_job(tenant_id, job_id, data_sync_api_job_v1_cancel_job_request=data_sync_api_job_v1_cancel_job_request)
    except Exception as e:
        print("Exception when calling JobsApi->cancel_tenant_data_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 
 **data_sync_api_job_v1_cancel_job_request** | [**DataSyncApiJobV1CancelJobRequest**](DataSyncApiJobV1CancelJobRequest.md)|  | [optional] 

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
**202** | The request has been accepted for processing, but the processing is not yet complete. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_job**
> ValidationsApiCoreV1CreatedResponse create_job(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_validations_create_validation_job_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_validations_create_validation_job_request)

Creates a Job.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_validations_create_validation_job_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsValidationsCreateValidationJobRequest
from edgraph_platform_client.models.validations_api_core_v1_created_response import ValidationsApiCoreV1CreatedResponse
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
    api_instance = edgraph_platform_client.JobsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_validations_create_validation_job_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsValidationsCreateValidationJobRequest() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsValidationsCreateValidationJobRequest |  (optional)

    try:
        # Creates a Job.
        api_response = api_instance.create_job(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_validations_create_validation_job_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_validations_create_validation_job_request)
        print("The response of JobsApi->create_job:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling JobsApi->create_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_validations_create_validation_job_request** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsValidationsCreateValidationJobRequest**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsValidationsCreateValidationJobRequest.md)|  | [optional] 

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
**201** | The resource was created. The location of the resource is available in the Location header of the response. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_tenant_data_sync_job**
> create_tenant_data_sync_job(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_create_job_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_create_job_request)

Creates a new DataSync job

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_create_job_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsCreateJobRequest
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
    api_instance = edgraph_platform_client.JobsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_create_job_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsCreateJobRequest() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsCreateJobRequest |  (optional)

    try:
        # Creates a new DataSync job
        api_instance.create_tenant_data_sync_job(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_create_job_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_create_job_request)
    except Exception as e:
        print("Exception when calling JobsApi->create_tenant_data_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_create_job_request** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsCreateJobRequest**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsCreateJobRequest.md)|  | [optional] 

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

# **deactivate_tenant_data_sync_job**
> deactivate_tenant_data_sync_job(tenant_id, job_id, data_sync_api_job_v1_deactivate_job_request=data_sync_api_job_v1_deactivate_job_request)

Deactivate a DataSync job matching the primary key

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_job_v1_deactivate_job_request import DataSyncApiJobV1DeactivateJobRequest
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
    api_instance = edgraph_platform_client.JobsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 
    data_sync_api_job_v1_deactivate_job_request = edgraph_platform_client.DataSyncApiJobV1DeactivateJobRequest() # DataSyncApiJobV1DeactivateJobRequest |  (optional)

    try:
        # Deactivate a DataSync job matching the primary key
        api_instance.deactivate_tenant_data_sync_job(tenant_id, job_id, data_sync_api_job_v1_deactivate_job_request=data_sync_api_job_v1_deactivate_job_request)
    except Exception as e:
        print("Exception when calling JobsApi->deactivate_tenant_data_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 
 **data_sync_api_job_v1_deactivate_job_request** | [**DataSyncApiJobV1DeactivateJobRequest**](DataSyncApiJobV1DeactivateJobRequest.md)|  | [optional] 

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
**202** | The request has been accepted for processing, but the processing is not yet complete. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_job**
> delete_job(tenant_id, job_id)

Deletes a Job.

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
    api_instance = edgraph_platform_client.JobsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 

    try:
        # Deletes a Job.
        api_instance.delete_job(tenant_id, job_id)
    except Exception as e:
        print("Exception when calling JobsApi->delete_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 

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

# **delete_tenant_data_sync_job**
> delete_tenant_data_sync_job(tenant_id, job_id)

Delete a DataSync job matching the primary key

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
    api_instance = edgraph_platform_client.JobsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 

    try:
        # Delete a DataSync job matching the primary key
        api_instance.delete_tenant_data_sync_job(tenant_id, job_id)
    except Exception as e:
        print("Exception when calling JobsApi->delete_tenant_data_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 

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

# **execute_job**
> object execute_job(tenant_id, job_id)

Requests a Job execution.

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
    api_instance = edgraph_platform_client.JobsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 

    try:
        # Requests a Job execution.
        api_response = api_instance.execute_job(tenant_id, job_id)
        print("The response of JobsApi->execute_job:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling JobsApi->execute_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 

### Return type

**object**

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

# **execute_tenant_data_sync_job**
> execute_tenant_data_sync_job(tenant_id, job_id, data_sync_api_job_v1_execute_job_request=data_sync_api_job_v1_execute_job_request)

Execute a DataSync job matching the primary key

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_job_v1_execute_job_request import DataSyncApiJobV1ExecuteJobRequest
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
    api_instance = edgraph_platform_client.JobsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 
    data_sync_api_job_v1_execute_job_request = edgraph_platform_client.DataSyncApiJobV1ExecuteJobRequest() # DataSyncApiJobV1ExecuteJobRequest |  (optional)

    try:
        # Execute a DataSync job matching the primary key
        api_instance.execute_tenant_data_sync_job(tenant_id, job_id, data_sync_api_job_v1_execute_job_request=data_sync_api_job_v1_execute_job_request)
    except Exception as e:
        print("Exception when calling JobsApi->execute_tenant_data_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 
 **data_sync_api_job_v1_execute_job_request** | [**DataSyncApiJobV1ExecuteJobRequest**](DataSyncApiJobV1ExecuteJobRequest.md)|  | [optional] 

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
**202** | The request has been accepted for processing, but the processing is not yet complete. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_all_tenant_data_sync_jobs**
> DataSyncApiJobV1JobListResponsePaginatedItemsViewModel get_all_tenant_data_sync_jobs(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of DataSync Jobs

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_job_v1_job_list_response_paginated_items_view_model import DataSyncApiJobV1JobListResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.JobsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of DataSync Jobs
        api_response = api_instance.get_all_tenant_data_sync_jobs(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of JobsApi->get_all_tenant_data_sync_jobs:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling JobsApi->get_all_tenant_data_sync_jobs: %s\n" % e)
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

[**DataSyncApiJobV1JobListResponsePaginatedItemsViewModel**](DataSyncApiJobV1JobListResponsePaginatedItemsViewModel.md)

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

# **get_job_by_id**
> ValidationsApiJobsV1JobProfileResponse get_job_by_id(tenant_id, job_id)

Retrieves a Job by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_jobs_v1_job_profile_response import ValidationsApiJobsV1JobProfileResponse
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
    api_instance = edgraph_platform_client.JobsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 

    try:
        # Retrieves a Job by ID.
        api_response = api_instance.get_job_by_id(tenant_id, job_id)
        print("The response of JobsApi->get_job_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling JobsApi->get_job_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 

### Return type

[**ValidationsApiJobsV1JobProfileResponse**](ValidationsApiJobsV1JobProfileResponse.md)

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

# **get_jobs**
> ValidationsApiJobsV1PaginatedItemsResponse get_jobs(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)

Retrieves a list of Jobs.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_jobs_v1_paginated_items_response import ValidationsApiJobsV1PaginatedItemsResponse
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
    api_instance = edgraph_platform_client.JobsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    filter = 'filter_example' # str |  (optional)
    order_by = 'order_by_example' # str |  (optional)

    try:
        # Retrieves a list of Jobs.
        api_response = api_instance.get_jobs(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)
        print("The response of JobsApi->get_jobs:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling JobsApi->get_jobs: %s\n" % e)
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

[**ValidationsApiJobsV1PaginatedItemsResponse**](ValidationsApiJobsV1PaginatedItemsResponse.md)

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

# **get_tenant_data_sync_job_profile_by_id**
> DataSyncApiJobV1JobProfileResponse get_tenant_data_sync_job_profile_by_id(tenant_id, job_id)

Retrieves a specific DataSync job using its primary key

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_job_v1_job_profile_response import DataSyncApiJobV1JobProfileResponse
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
    api_instance = edgraph_platform_client.JobsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 

    try:
        # Retrieves a specific DataSync job using its primary key
        api_response = api_instance.get_tenant_data_sync_job_profile_by_id(tenant_id, job_id)
        print("The response of JobsApi->get_tenant_data_sync_job_profile_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling JobsApi->get_tenant_data_sync_job_profile_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 

### Return type

[**DataSyncApiJobV1JobProfileResponse**](DataSyncApiJobV1JobProfileResponse.md)

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

# **restart_job_schedule**
> restart_job_schedule(tenant_id, job_id)

Requests a Job schedule restart.

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
    api_instance = edgraph_platform_client.JobsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 

    try:
        # Requests a Job schedule restart.
        api_instance.restart_job_schedule(tenant_id, job_id)
    except Exception as e:
        print("Exception when calling JobsApi->restart_job_schedule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 

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
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_job**
> update_job(tenant_id, job_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_validation_job_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_validation_job_request)

Updates a Job.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_validation_job_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsUpdateValidationJobRequest
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
    api_instance = edgraph_platform_client.JobsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_validation_job_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsUpdateValidationJobRequest() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsUpdateValidationJobRequest |  (optional)

    try:
        # Updates a Job.
        api_instance.update_job(tenant_id, job_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_validation_job_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_validation_job_request)
    except Exception as e:
        print("Exception when calling JobsApi->update_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_validation_job_request** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsUpdateValidationJobRequest**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsUpdateValidationJobRequest.md)|  | [optional] 

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_tenant_data_sync_job**
> update_tenant_data_sync_job(tenant_id, job_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_job_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_job_request)

Updates a DataSync job matching the primary key

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_job_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsUpdateJobRequest
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
    api_instance = edgraph_platform_client.JobsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_job_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsUpdateJobRequest() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsUpdateJobRequest |  (optional)

    try:
        # Updates a DataSync job matching the primary key
        api_instance.update_tenant_data_sync_job(tenant_id, job_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_job_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_job_request)
    except Exception as e:
        print("Exception when calling JobsApi->update_tenant_data_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_job_request** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsUpdateJobRequest**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsUpdateJobRequest.md)|  | [optional] 

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
**202** | The request has been accepted for processing, but the processing is not yet complete. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

