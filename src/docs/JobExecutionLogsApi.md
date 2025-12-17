# edgraph_platform_client.JobExecutionLogsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_all_tenant_data_sync_job_execution_logs**](JobExecutionLogsApi.md#get_all_tenant_data_sync_job_execution_logs) | **GET** /tenants/{tenantId}/datasync/jobs/{jobId}/executions/{jobExecutionId}/logs | Retrieves a list of DataSync Job Execution Logs


# **get_all_tenant_data_sync_job_execution_logs**
> DataSyncApiJobExecutionLogV1JobExecutionLogEntryPaginatedItemsViewModel get_all_tenant_data_sync_job_execution_logs(tenant_id, job_id, job_execution_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter, search=search)

Retrieves a list of DataSync Job Execution Logs

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_job_execution_log_v1_job_execution_log_entry_paginated_items_view_model import DataSyncApiJobExecutionLogV1JobExecutionLogEntryPaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.JobExecutionLogsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 
    job_execution_id = 'job_execution_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')
    search = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of DataSync Job Execution Logs
        api_response = api_instance.get_all_tenant_data_sync_job_execution_logs(tenant_id, job_id, job_execution_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter, search=search)
        print("The response of JobExecutionLogsApi->get_all_tenant_data_sync_job_execution_logs:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling JobExecutionLogsApi->get_all_tenant_data_sync_job_execution_logs: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 
 **job_execution_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]
 **search** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**DataSyncApiJobExecutionLogV1JobExecutionLogEntryPaginatedItemsViewModel**](DataSyncApiJobExecutionLogV1JobExecutionLogEntryPaginatedItemsViewModel.md)

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

