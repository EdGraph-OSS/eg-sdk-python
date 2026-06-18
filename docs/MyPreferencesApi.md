# edgraph_platform_client.MyPreferencesApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_user_preferences**](MyPreferencesApi.md#get_user_preferences) | **GET** /me/preferences | Retrieves the user&#39;s preferences.
[**preference**](MyPreferencesApi.md#preference) | **GET** /me/preferences/{code} | Retrieves a user&#39;s preference by code.
[**update_user_preference_async**](MyPreferencesApi.md#update_user_preference_async) | **POST** /me/preferences | Creates or update a user&#39;s preference.


# **get_user_preferences**
> IdentityApiUserV1GetUserPreferencesResponse get_user_preferences(page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)

Retrieves the user's preferences.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v1_get_user_preferences_response import IdentityApiUserV1GetUserPreferencesResponse
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
    api_instance = edgraph_platform_client.MyPreferencesApi(api_client)
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = 'order_by_example' # str |  (optional)
    filter = 'filter_example' # str |  (optional)

    try:
        # Retrieves the user's preferences.
        api_response = await api_instance.get_user_preferences(page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)
        print("The response of MyPreferencesApi->get_user_preferences:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MyPreferencesApi->get_user_preferences: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **order_by** | **str**|  | [optional] 
 **filter** | **str**|  | [optional] 

### Return type

[**IdentityApiUserV1GetUserPreferencesResponse**](IdentityApiUserV1GetUserPreferencesResponse.md)

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

# **preference**
> EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheResponse preference(code)

Retrieves a user's preference by code.

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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.MyPreferencesApi(api_client)
    code = 'code_example' # str | 

    try:
        # Retrieves a user's preference by code.
        api_response = await api_instance.preference(code)
        print("The response of MyPreferencesApi->preference:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MyPreferencesApi->preference: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **code** | **str**|  | 

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

# **update_user_preference_async**
> IdentityApiUserV1UserPreferenceUpdatedResponse update_user_preference_async(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_update_user_preference_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_update_user_preference_request)

Creates or update a user's preference.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_update_user_preference_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsUpdateUserPreferenceRequest
from edgraph_platform_client.models.identity_api_user_v1_user_preference_updated_response import IdentityApiUserV1UserPreferenceUpdatedResponse
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
    api_instance = edgraph_platform_client.MyPreferencesApi(api_client)
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_update_user_preference_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsUpdateUserPreferenceRequest() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsUpdateUserPreferenceRequest |  (optional)

    try:
        # Creates or update a user's preference.
        api_response = await api_instance.update_user_preference_async(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_update_user_preference_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_update_user_preference_request)
        print("The response of MyPreferencesApi->update_user_preference_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MyPreferencesApi->update_user_preference_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_update_user_preference_request** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsUpdateUserPreferenceRequest**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsUpdateUserPreferenceRequest.md)|  | [optional] 

### Return type

[**IdentityApiUserV1UserPreferenceUpdatedResponse**](IdentityApiUserV1UserPreferenceUpdatedResponse.md)

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

