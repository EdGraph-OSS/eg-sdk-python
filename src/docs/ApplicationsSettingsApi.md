# edgraph_platform_client.ApplicationsSettingsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_client_settings_async**](ApplicationsSettingsApi.md#get_client_settings_async) | **GET** /tenants/{tenantId}/clients/{clientId}/settings | Retrieves a list of a Tenant&#39;s ClientSettings.
[**get_client_settings_types_async**](ApplicationsSettingsApi.md#get_client_settings_types_async) | **GET** /tenants/{tenantId}/clients/{clientId}/settingstypes | Retrieves a list of ClientSettingsTypes.
[**set_client_settings_async**](ApplicationsSettingsApi.md#set_client_settings_async) | **POST** /tenants/{tenantId}/clients/{clientId}/settings | Creates/updates a Tenant&#39;s ClientSettings.


# **get_client_settings_async**
> TenantApiTenantV1GetAppSettingsResponse get_client_settings_async(tenant_id, client_id)

Retrieves a list of a Tenant's ClientSettings.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_tenant_v1_get_app_settings_response import TenantApiTenantV1GetAppSettingsResponse
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
    api_instance = edgraph_platform_client.ApplicationsSettingsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    client_id = 'client_id_example' # str | 

    try:
        # Retrieves a list of a Tenant's ClientSettings.
        api_response = api_instance.get_client_settings_async(tenant_id, client_id)
        print("The response of ApplicationsSettingsApi->get_client_settings_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApplicationsSettingsApi->get_client_settings_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **client_id** | **str**|  | 

### Return type

[**TenantApiTenantV1GetAppSettingsResponse**](TenantApiTenantV1GetAppSettingsResponse.md)

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

# **get_client_settings_types_async**
> IdentityApiClientSettingsTypeV1GetClientSettingsTypesResponse get_client_settings_types_async(tenant_id, client_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)

Retrieves a list of ClientSettingsTypes.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_client_settings_type_v1_get_client_settings_types_response import IdentityApiClientSettingsTypeV1GetClientSettingsTypesResponse
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
    api_instance = edgraph_platform_client.ApplicationsSettingsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    client_id = 'client_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of ClientSettingsTypes.
        api_response = api_instance.get_client_settings_types_async(tenant_id, client_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)
        print("The response of ApplicationsSettingsApi->get_client_settings_types_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApplicationsSettingsApi->get_client_settings_types_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **client_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**IdentityApiClientSettingsTypeV1GetClientSettingsTypesResponse**](IdentityApiClientSettingsTypeV1GetClientSettingsTypesResponse.md)

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

# **set_client_settings_async**
> TenantApiTenantV1SetAppSettingsResponse set_client_settings_async(tenant_id, client_id, tenant_api_tenant_v1_set_app_settings_request=tenant_api_tenant_v1_set_app_settings_request)

Creates/updates a Tenant's ClientSettings.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_tenant_v1_set_app_settings_request import TenantApiTenantV1SetAppSettingsRequest
from edgraph_platform_client.models.tenant_api_tenant_v1_set_app_settings_response import TenantApiTenantV1SetAppSettingsResponse
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
    api_instance = edgraph_platform_client.ApplicationsSettingsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    client_id = 'client_id_example' # str | 
    tenant_api_tenant_v1_set_app_settings_request = edgraph_platform_client.TenantApiTenantV1SetAppSettingsRequest() # TenantApiTenantV1SetAppSettingsRequest |  (optional)

    try:
        # Creates/updates a Tenant's ClientSettings.
        api_response = api_instance.set_client_settings_async(tenant_id, client_id, tenant_api_tenant_v1_set_app_settings_request=tenant_api_tenant_v1_set_app_settings_request)
        print("The response of ApplicationsSettingsApi->set_client_settings_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApplicationsSettingsApi->set_client_settings_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **client_id** | **str**|  | 
 **tenant_api_tenant_v1_set_app_settings_request** | [**TenantApiTenantV1SetAppSettingsRequest**](TenantApiTenantV1SetAppSettingsRequest.md)|  | [optional] 

### Return type

[**TenantApiTenantV1SetAppSettingsResponse**](TenantApiTenantV1SetAppSettingsResponse.md)

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

