# edgraph_platform_client.MyTenantsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_user_tenants**](MyTenantsApi.md#get_user_tenants) | **GET** /me/tenants | Retrieves the Tenants of the User that is currently logged in.
[**search_my_licenses**](MyTenantsApi.md#search_my_licenses) | **GET** /v2/me/tenants/{tenantId}/licenses | Search the user&#39;s licenses.
[**search_my_tenants**](MyTenantsApi.md#search_my_tenants) | **GET** /v2/me/tenants | Searches tenants associated to the user.


# **get_user_tenants**
> IdentityApiUserV1UserTenantProfilePaginatedItemsViewModel get_user_tenants(page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)

Retrieves the Tenants of the User that is currently logged in.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v1_user_tenant_profile_paginated_items_view_model import IdentityApiUserV1UserTenantProfilePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.MyTenantsApi(api_client)
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    filter = '' # str |  (optional) (default to '')
    order_by = '' # str |  (optional) (default to '')

    try:
        # Retrieves the Tenants of the User that is currently logged in.
        api_response = api_instance.get_user_tenants(page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)
        print("The response of MyTenantsApi->get_user_tenants:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MyTenantsApi->get_user_tenants: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**IdentityApiUserV1UserTenantProfilePaginatedItemsViewModel**](IdentityApiUserV1UserTenantProfilePaginatedItemsViewModel.md)

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

# **search_my_licenses**
> IdentityApiUserV2UserMeTenantsResponsePaginatedItemsViewModel search_my_licenses(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)

Search the user's licenses.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v2_user_me_tenants_response_paginated_items_view_model import IdentityApiUserV2UserMeTenantsResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.MyTenantsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    filter = '' # str |  (optional) (default to '')
    order_by = '' # str |  (optional) (default to '')

    try:
        # Search the user's licenses.
        api_response = api_instance.search_my_licenses(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)
        print("The response of MyTenantsApi->search_my_licenses:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MyTenantsApi->search_my_licenses: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**IdentityApiUserV2UserMeTenantsResponsePaginatedItemsViewModel**](IdentityApiUserV2UserMeTenantsResponsePaginatedItemsViewModel.md)

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

# **search_my_tenants**
> IdentityApiUserV2UserMeTenantsResponsePaginatedItemsViewModel search_my_tenants(page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)

Searches tenants associated to the user.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v2_user_me_tenants_response_paginated_items_view_model import IdentityApiUserV2UserMeTenantsResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.MyTenantsApi(api_client)
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    filter = '' # str |  (optional) (default to '')
    order_by = '' # str |  (optional) (default to '')

    try:
        # Searches tenants associated to the user.
        api_response = api_instance.search_my_tenants(page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)
        print("The response of MyTenantsApi->search_my_tenants:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MyTenantsApi->search_my_tenants: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**IdentityApiUserV2UserMeTenantsResponsePaginatedItemsViewModel**](IdentityApiUserV2UserMeTenantsResponsePaginatedItemsViewModel.md)

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

