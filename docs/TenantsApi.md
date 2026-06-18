# edgraph_platform_client.TenantsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_tenant_by_id_async**](TenantsApi.md#get_tenant_by_id_async) | **GET** /tenants/{tenantId} | Retrieves the profile of a specific tenant
[**update_tenant_async**](TenantsApi.md#update_tenant_async) | **PUT** /tenants/{tenantId} | Updates a tenant&#39;s profile


# **get_tenant_by_id_async**
> TenantApiTenantV1TenantProfileResponse get_tenant_by_id_async(tenant_id)

Retrieves the profile of a specific tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_tenant_v1_tenant_profile_response import TenantApiTenantV1TenantProfileResponse
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
    api_instance = edgraph_platform_client.TenantsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 

    try:
        # Retrieves the profile of a specific tenant
        api_response = await api_instance.get_tenant_by_id_async(tenant_id)
        print("The response of TenantsApi->get_tenant_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantsApi->get_tenant_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 

### Return type

[**TenantApiTenantV1TenantProfileResponse**](TenantApiTenantV1TenantProfileResponse.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_tenant_async**
> TenantApiTenantV1TenantUpdatedResponse update_tenant_async(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_update_tenant_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_update_tenant_request)

Updates a tenant's profile

Note: Only the tenant's Identity Providers can be updated at this time

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_update_tenant_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsUpdateTenantRequest
from edgraph_platform_client.models.tenant_api_tenant_v1_tenant_updated_response import TenantApiTenantV1TenantUpdatedResponse
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
    api_instance = edgraph_platform_client.TenantsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_update_tenant_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsUpdateTenantRequest() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsUpdateTenantRequest |  (optional)

    try:
        # Updates a tenant's profile
        api_response = await api_instance.update_tenant_async(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_update_tenant_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_update_tenant_request)
        print("The response of TenantsApi->update_tenant_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantsApi->update_tenant_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_update_tenant_request** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsUpdateTenantRequest**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsUpdateTenantRequest.md)|  | [optional] 

### Return type

[**TenantApiTenantV1TenantUpdatedResponse**](TenantApiTenantV1TenantUpdatedResponse.md)

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

