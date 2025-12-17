# edgraph_platform_client.MyProfileApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_my_profile**](MyProfileApi.md#get_my_profile) | **GET** /v2/me | Get the profile of the user that is currently logged in.
[**get_my_tenant**](MyProfileApi.md#get_my_tenant) | **GET** /v2/me/tenants/{tenantId} | Get the tenant associated to the user.
[**get_user_cache_async**](MyProfileApi.md#get_user_cache_async) | **GET** /me | Retrieves the profile of the user that is currently logged in, including the user&#39;s preferences and its associated tenants


# **get_my_profile**
> IdentityApiUserV2UserMeProfile get_my_profile()

Get the profile of the user that is currently logged in.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v2_user_me_profile import IdentityApiUserV2UserMeProfile
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
    api_instance = edgraph_platform_client.MyProfileApi(api_client)

    try:
        # Get the profile of the user that is currently logged in.
        api_response = api_instance.get_my_profile()
        print("The response of MyProfileApi->get_my_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MyProfileApi->get_my_profile: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**IdentityApiUserV2UserMeProfile**](IdentityApiUserV2UserMeProfile.md)

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

# **get_my_tenant**
> IdentityApiUserV2TenantMeProfile get_my_tenant(tenant_id)

Get the tenant associated to the user.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v2_tenant_me_profile import IdentityApiUserV2TenantMeProfile
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
    api_instance = edgraph_platform_client.MyProfileApi(api_client)
    tenant_id = 'tenant_id_example' # str | 

    try:
        # Get the tenant associated to the user.
        api_response = api_instance.get_my_tenant(tenant_id)
        print("The response of MyProfileApi->get_my_tenant:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MyProfileApi->get_my_tenant: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 

### Return type

[**IdentityApiUserV2TenantMeProfile**](IdentityApiUserV2TenantMeProfile.md)

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

# **get_user_cache_async**
> EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheResponse get_user_cache_async(number_of_tenants=number_of_tenants)

Retrieves the profile of the user that is currently logged in, including the user's preferences and its associated tenants

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_cache_response import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheResponse
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
    api_instance = edgraph_platform_client.MyProfileApi(api_client)
    number_of_tenants = 10 # int |  (optional) (default to 10)

    try:
        # Retrieves the profile of the user that is currently logged in, including the user's preferences and its associated tenants
        api_response = api_instance.get_user_cache_async(number_of_tenants=number_of_tenants)
        print("The response of MyProfileApi->get_user_cache_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MyProfileApi->get_user_cache_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **number_of_tenants** | **int**|  | [optional] [default to 10]

### Return type

[**EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheResponse**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheResponse.md)

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

