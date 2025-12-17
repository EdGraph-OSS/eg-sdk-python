# edgraph_platform_client.InstancesLogsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_instance_http_logs**](InstancesLogsApi.md#get_instance_http_logs) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/logs/http | Retrieves HTTP logs for a given instance


# **get_instance_http_logs**
> EdGraphHttpAggregatorsTenantApiServicesEdFiAdminUseCasesInstanceLogPaginatedItemsViewModel get_instance_http_logs(tenant_id, instance_id, year, page_size=page_size, page_index=page_index, var_from=var_from, to=to, var_field=var_field, order=order)

Retrieves HTTP logs for a given instance

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_ed_fi_admin_use_cases_instance_log_paginated_items_view_model import EdGraphHttpAggregatorsTenantApiServicesEdFiAdminUseCasesInstanceLogPaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.InstancesLogsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    var_from = 0 # int |  (optional) (default to 0)
    to = 0 # int |  (optional) (default to 0)
    var_field = '' # str |  (optional) (default to '')
    order = False # bool |  (optional) (default to False)

    try:
        # Retrieves HTTP logs for a given instance
        api_response = api_instance.get_instance_http_logs(tenant_id, instance_id, year, page_size=page_size, page_index=page_index, var_from=var_from, to=to, var_field=var_field, order=order)
        print("The response of InstancesLogsApi->get_instance_http_logs:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesLogsApi->get_instance_http_logs: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **var_from** | **int**|  | [optional] [default to 0]
 **to** | **int**|  | [optional] [default to 0]
 **var_field** | **str**|  | [optional] [default to &#39;&#39;]
 **order** | **bool**|  | [optional] [default to False]

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesEdFiAdminUseCasesInstanceLogPaginatedItemsViewModel**](EdGraphHttpAggregatorsTenantApiServicesEdFiAdminUseCasesInstanceLogPaginatedItemsViewModel.md)

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

