# edgraph_platform_client.ApplicationsTilesApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_tenant_application_tiles_async**](ApplicationsTilesApi.md#get_tenant_application_tiles_async) | **GET** /tenants/{tenantId}/applicationtiles | Retrieves a list of applications licensed to the user that is currently logged in the context of this tenant


# **get_tenant_application_tiles_async**
> EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesApplicationTilesResponseWithUserApplicationLicense get_tenant_application_tiles_async(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)

Retrieves a list of applications licensed to the user that is currently logged in the context of this tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_application_tiles_response_with_user_application_license import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesApplicationTilesResponseWithUserApplicationLicense
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
    api_instance = edgraph_platform_client.ApplicationsTilesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 100 # int |  (optional) (default to 100)
    order_by = 'applicationName ASC' # str |  (optional) (default to 'applicationName ASC')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of applications licensed to the user that is currently logged in the context of this tenant
        api_response = api_instance.get_tenant_application_tiles_async(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)
        print("The response of ApplicationsTilesApi->get_tenant_application_tiles_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApplicationsTilesApi->get_tenant_application_tiles_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 100]
 **order_by** | **str**|  | [optional] [default to &#39;applicationName ASC&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesApplicationTilesResponseWithUserApplicationLicense**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesApplicationTilesResponseWithUserApplicationLicense.md)

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

