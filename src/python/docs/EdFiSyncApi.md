# edgraph_platform_client.EdFiSyncApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_ed_fi_sync**](EdFiSyncApi.md#create_ed_fi_sync) | **POST** /tenants/{tenantId}/jobs/edfisync | Creates an Ed-Fi Sync Job for a given tenant
[**execute_ed_fi_sync_job**](EdFiSyncApi.md#execute_ed_fi_sync_job) | **PUT** /tenants/{tenantId}/jobs/edfisync/execute | Executes an Ed-Fi Sync Job
[**get_ed_fi_sync_data**](EdFiSyncApi.md#get_ed_fi_sync_data) | **GET** /tenants/{tenantId}/jobs/edfisync | Retrieves Ed-Fi Sync Connection Data for a given tenant
[**update_ed_fi_sync**](EdFiSyncApi.md#update_ed_fi_sync) | **PUT** /tenants/{tenantId}/jobs/edfisync | Updates an Ed-Fi Sync for a given tenant


# **create_ed_fi_sync**
> EdGraphHttpAggregatorsTenantApiServicesEdFiRosterSyncJobCreatedResult create_ed_fi_sync(tenant_id, ed_graph_http_aggregators_tenant_api_services_ed_fi_roster_sync_create_ed_fi_roster_sync_job_request_dto=ed_graph_http_aggregators_tenant_api_services_ed_fi_roster_sync_create_ed_fi_roster_sync_job_request_dto)

Creates an Ed-Fi Sync Job for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_ed_fi_roster_sync_create_ed_fi_roster_sync_job_request_dto import EdGraphHttpAggregatorsTenantApiServicesEdFiRosterSyncCreateEdFiRosterSyncJobRequestDto
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_ed_fi_roster_sync_job_created_result import EdGraphHttpAggregatorsTenantApiServicesEdFiRosterSyncJobCreatedResult
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
    api_instance = edgraph_platform_client.EdFiSyncApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_services_ed_fi_roster_sync_create_ed_fi_roster_sync_job_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesEdFiRosterSyncCreateEdFiRosterSyncJobRequestDto() # EdGraphHttpAggregatorsTenantApiServicesEdFiRosterSyncCreateEdFiRosterSyncJobRequestDto |  (optional)

    try:
        # Creates an Ed-Fi Sync Job for a given tenant
        api_response = api_instance.create_ed_fi_sync(tenant_id, ed_graph_http_aggregators_tenant_api_services_ed_fi_roster_sync_create_ed_fi_roster_sync_job_request_dto=ed_graph_http_aggregators_tenant_api_services_ed_fi_roster_sync_create_ed_fi_roster_sync_job_request_dto)
        print("The response of EdFiSyncApi->create_ed_fi_sync:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EdFiSyncApi->create_ed_fi_sync: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_services_ed_fi_roster_sync_create_ed_fi_roster_sync_job_request_dto** | [**EdGraphHttpAggregatorsTenantApiServicesEdFiRosterSyncCreateEdFiRosterSyncJobRequestDto**](EdGraphHttpAggregatorsTenantApiServicesEdFiRosterSyncCreateEdFiRosterSyncJobRequestDto.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesEdFiRosterSyncJobCreatedResult**](EdGraphHttpAggregatorsTenantApiServicesEdFiRosterSyncJobCreatedResult.md)

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

# **execute_ed_fi_sync_job**
> DataSyncApiJobV1JobExecutionRequestedResponse execute_ed_fi_sync_job(tenant_id)

Executes an Ed-Fi Sync Job

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_job_v1_job_execution_requested_response import DataSyncApiJobV1JobExecutionRequestedResponse
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
    api_instance = edgraph_platform_client.EdFiSyncApi(api_client)
    tenant_id = 'tenant_id_example' # str | 

    try:
        # Executes an Ed-Fi Sync Job
        api_response = api_instance.execute_ed_fi_sync_job(tenant_id)
        print("The response of EdFiSyncApi->execute_ed_fi_sync_job:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EdFiSyncApi->execute_ed_fi_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 

### Return type

[**DataSyncApiJobV1JobExecutionRequestedResponse**](DataSyncApiJobV1JobExecutionRequestedResponse.md)

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

# **get_ed_fi_sync_data**
> DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobProfile get_ed_fi_sync_data(tenant_id)

Retrieves Ed-Fi Sync Connection Data for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_ed_fi_roster_sync_v1_ed_fi_roster_sync_job_profile import DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobProfile
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
    api_instance = edgraph_platform_client.EdFiSyncApi(api_client)
    tenant_id = 'tenant_id_example' # str | 

    try:
        # Retrieves Ed-Fi Sync Connection Data for a given tenant
        api_response = api_instance.get_ed_fi_sync_data(tenant_id)
        print("The response of EdFiSyncApi->get_ed_fi_sync_data:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EdFiSyncApi->get_ed_fi_sync_data: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 

### Return type

[**DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobProfile**](DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobProfile.md)

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

# **update_ed_fi_sync**
> MicrosoftAspNetCoreMvcNoContentResult update_ed_fi_sync(tenant_id, body=body)

Updates an Ed-Fi Sync for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
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
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.EdFiSyncApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    body = None # object |  (optional)

    try:
        # Updates an Ed-Fi Sync for a given tenant
        api_response = api_instance.update_ed_fi_sync(tenant_id, body=body)
        print("The response of EdFiSyncApi->update_ed_fi_sync:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EdFiSyncApi->update_ed_fi_sync: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **body** | **object**|  | [optional] 

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
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

