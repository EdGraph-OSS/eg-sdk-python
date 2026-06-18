# edgraph_platform_client.TenantBrandingApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**update_tenant_branding**](TenantBrandingApi.md#update_tenant_branding) | **PUT** /tenants/{tenantId}/branding | Updates the branding of tenant


# **update_tenant_branding**
> TenantApiTenantV1TenantUpdatedResponse update_tenant_branding(tenant_id, logo_file=logo_file, background_file=background_file, brand_name=brand_name, enabled=enabled)

Updates the branding of tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
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
    api_instance = edgraph_platform_client.TenantBrandingApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    logo_file = None # bytes |  (optional)
    background_file = None # bytes |  (optional)
    brand_name = 'brand_name_example' # str |  (optional)
    enabled = True # bool |  (optional)

    try:
        # Updates the branding of tenant
        api_response = await api_instance.update_tenant_branding(tenant_id, logo_file=logo_file, background_file=background_file, brand_name=brand_name, enabled=enabled)
        print("The response of TenantBrandingApi->update_tenant_branding:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantBrandingApi->update_tenant_branding: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **logo_file** | **bytes**|  | [optional] 
 **background_file** | **bytes**|  | [optional] 
 **brand_name** | **str**|  | [optional] 
 **enabled** | **bool**|  | [optional] 

### Return type

[**TenantApiTenantV1TenantUpdatedResponse**](TenantApiTenantV1TenantUpdatedResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**200** | The requested resource was successfully retrieved. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

