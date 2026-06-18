# edgraph_platform_client.LogsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_logs**](LogsApi.md#get_logs) | **GET** /tenants/{tenantId}/validations/logs | Retrieves a list of Logs.


# **get_logs**
> ValidationsApiValidationResultsV1FindResponse get_logs(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, environment_id=environment_id, collection_id=collection_id, container_id=container_id, rule_id=rule_id, job_id=job_id, job_execution_id=job_execution_id)

Retrieves a list of Logs.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_validation_results_v1_find_response import ValidationsApiValidationResultsV1FindResponse
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
    api_instance = edgraph_platform_client.LogsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = 'order_by_example' # str |  (optional)
    environment_id = 'environment_id_example' # str |  (optional)
    collection_id = 'collection_id_example' # str |  (optional)
    container_id = 'container_id_example' # str |  (optional)
    rule_id = 'rule_id_example' # str |  (optional)
    job_id = 'job_id_example' # str |  (optional)
    job_execution_id = 'job_execution_id_example' # str |  (optional)

    try:
        # Retrieves a list of Logs.
        api_response = await api_instance.get_logs(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, environment_id=environment_id, collection_id=collection_id, container_id=container_id, rule_id=rule_id, job_id=job_id, job_execution_id=job_execution_id)
        print("The response of LogsApi->get_logs:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LogsApi->get_logs: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **order_by** | **str**|  | [optional] 
 **environment_id** | **str**|  | [optional] 
 **collection_id** | **str**|  | [optional] 
 **container_id** | **str**|  | [optional] 
 **rule_id** | **str**|  | [optional] 
 **job_id** | **str**|  | [optional] 
 **job_execution_id** | **str**|  | [optional] 

### Return type

[**ValidationsApiValidationResultsV1FindResponse**](ValidationsApiValidationResultsV1FindResponse.md)

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

