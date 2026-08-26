# edgraph_platform_client.ClientBrandingApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_client_branding_async**](ClientBrandingApi.md#get_client_branding_async) | **GET** /clients/{clientId}/branding | Public (unauthenticated) read of a client&#39;s branding for the sign-in and other pre-auth  surfaces (Azure DevOps #17086). Returns only render fields + the override flag — never secrets,  storage internals, or other client configuration.


# **get_client_branding_async**
> EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesClientBrandingResponse get_client_branding_async(client_id)

Public (unauthenticated) read of a client's branding for the sign-in and other pre-auth  surfaces (Azure DevOps #17086). Returns only render fields + the override flag — never secrets,  storage internals, or other client configuration.

Unauthenticated by design (branding is shown before login). An unknown client returns a
disabled default rather than 404, so the endpoint cannot be used as a client-existence oracle.
The response is cacheable so downstream CDNs/browsers absorb most traffic; rate limiting is
expected at the gateway.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_client_branding_response import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesClientBrandingResponse
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
    api_instance = edgraph_platform_client.ClientBrandingApi(api_client)
    client_id = 'client_id_example' # str | The OAuth client id (already URL-decoded by routing).

    try:
        # Public (unauthenticated) read of a client's branding for the sign-in and other pre-auth  surfaces (Azure DevOps #17086). Returns only render fields + the override flag — never secrets,  storage internals, or other client configuration.
        api_response = await api_instance.get_client_branding_async(client_id)
        print("The response of ClientBrandingApi->get_client_branding_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ClientBrandingApi->get_client_branding_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **client_id** | **str**| The OAuth client id (already URL-decoded by routing). | 

### Return type

[**EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesClientBrandingResponse**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesClientBrandingResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**500** | An unhandled error occurred on the server. See the response body for details. |  -  |
**200** | The client&#39;s branding (or a disabled default for an unknown client). |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

