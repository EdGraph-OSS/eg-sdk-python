# edgraph_platform_client.MySettingsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_my_setting**](MySettingsApi.md#create_my_setting) | **POST** /me/settings | Create a User-scope setting
[**delete_my_setting**](MySettingsApi.md#delete_my_setting) | **DELETE** /me/settings/{settingIdOrCode} | Delete the User-scope setting for a key, addressed by SettingType id or Code
[**get_my_setting**](MySettingsApi.md#get_my_setting) | **GET** /me/settings/{settingIdOrCode} | Get a User-scope setting
[**search_my_settings**](MySettingsApi.md#search_my_settings) | **GET** /me/settings | List User-scope settings
[**set_my_setting**](MySettingsApi.md#set_my_setting) | **PUT** /me/settings | Create or update (upsert) a User-scope setting, addressed by the SettingTypeId in the body
[**update_my_setting**](MySettingsApi.md#update_my_setting) | **PUT** /me/settings/{settingIdOrCode} | Update the User-scope setting for a key, addressed by SettingType id or Code


# **create_my_setting**
> SettingsApiUserSettingsV1CreateUserSettingResponse create_my_setting(ed_graph_platform_http_aggregators_tenant_api_controllers_v1_create_my_setting_request_body=ed_graph_platform_http_aggregators_tenant_api_controllers_v1_create_my_setting_request_body)

Create a User-scope setting

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_create_my_setting_request_body import EdGraphPlatformHttpAggregatorsTenantApiControllersV1CreateMySettingRequestBody
from edgraph_platform_client.models.settings_api_user_settings_v1_create_user_setting_response import SettingsApiUserSettingsV1CreateUserSettingResponse
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
    api_instance = edgraph_platform_client.MySettingsApi(api_client)
    ed_graph_platform_http_aggregators_tenant_api_controllers_v1_create_my_setting_request_body = edgraph_platform_client.EdGraphPlatformHttpAggregatorsTenantApiControllersV1CreateMySettingRequestBody() # EdGraphPlatformHttpAggregatorsTenantApiControllersV1CreateMySettingRequestBody |  (optional)

    try:
        # Create a User-scope setting
        api_response = await api_instance.create_my_setting(ed_graph_platform_http_aggregators_tenant_api_controllers_v1_create_my_setting_request_body=ed_graph_platform_http_aggregators_tenant_api_controllers_v1_create_my_setting_request_body)
        print("The response of MySettingsApi->create_my_setting:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MySettingsApi->create_my_setting: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ed_graph_platform_http_aggregators_tenant_api_controllers_v1_create_my_setting_request_body** | [**EdGraphPlatformHttpAggregatorsTenantApiControllersV1CreateMySettingRequestBody**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1CreateMySettingRequestBody.md)|  | [optional] 

### Return type

[**SettingsApiUserSettingsV1CreateUserSettingResponse**](SettingsApiUserSettingsV1CreateUserSettingResponse.md)

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
**201** | Created |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_my_setting**
> delete_my_setting(setting_id_or_code, ed_graph_platform_http_aggregators_tenant_api_controllers_v1_delete_my_setting_request_body=ed_graph_platform_http_aggregators_tenant_api_controllers_v1_delete_my_setting_request_body)

Delete the User-scope setting for a key, addressed by SettingType id or Code

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_delete_my_setting_request_body import EdGraphPlatformHttpAggregatorsTenantApiControllersV1DeleteMySettingRequestBody
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
    api_instance = edgraph_platform_client.MySettingsApi(api_client)
    setting_id_or_code = 'setting_id_or_code_example' # str | 
    ed_graph_platform_http_aggregators_tenant_api_controllers_v1_delete_my_setting_request_body = edgraph_platform_client.EdGraphPlatformHttpAggregatorsTenantApiControllersV1DeleteMySettingRequestBody() # EdGraphPlatformHttpAggregatorsTenantApiControllersV1DeleteMySettingRequestBody |  (optional)

    try:
        # Delete the User-scope setting for a key, addressed by SettingType id or Code
        await api_instance.delete_my_setting(setting_id_or_code, ed_graph_platform_http_aggregators_tenant_api_controllers_v1_delete_my_setting_request_body=ed_graph_platform_http_aggregators_tenant_api_controllers_v1_delete_my_setting_request_body)
    except Exception as e:
        print("Exception when calling MySettingsApi->delete_my_setting: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **setting_id_or_code** | **str**|  | 
 **ed_graph_platform_http_aggregators_tenant_api_controllers_v1_delete_my_setting_request_body** | [**EdGraphPlatformHttpAggregatorsTenantApiControllersV1DeleteMySettingRequestBody**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1DeleteMySettingRequestBody.md)|  | [optional] 

### Return type

void (empty response body)

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
**204** | No Content |  -  |
**404** | Not Found |  -  |
**422** | Client Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_my_setting**
> SettingsApiUserSettingsV1UserSettingMessage get_my_setting(setting_id_or_code, setting_type_id=setting_type_id, provider=provider, application_id=application_id, resolve_effective_value=resolve_effective_value)

Get a User-scope setting

Answers with the stored record alone. Effective-value resolution is opt-in: pass
`resolveEffectiveValue=true` to instead receive the value in force at this scope — every
layer above it merged under the setting's own value.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.settings_api_user_settings_v1_user_setting_message import SettingsApiUserSettingsV1UserSettingMessage
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
    api_instance = edgraph_platform_client.MySettingsApi(api_client)
    setting_id_or_code = 'setting_id_or_code_example' # str | 
    setting_type_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID |  (optional)
    provider = 'provider_example' # str |  (optional)
    application_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID |  (optional)
    resolve_effective_value = False # bool |  (optional) (default to False)

    try:
        # Get a User-scope setting
        api_response = await api_instance.get_my_setting(setting_id_or_code, setting_type_id=setting_type_id, provider=provider, application_id=application_id, resolve_effective_value=resolve_effective_value)
        print("The response of MySettingsApi->get_my_setting:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MySettingsApi->get_my_setting: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **setting_id_or_code** | **str**|  | 
 **setting_type_id** | **UUID**|  | [optional] 
 **provider** | **str**|  | [optional] 
 **application_id** | **UUID**|  | [optional] 
 **resolve_effective_value** | **bool**|  | [optional] [default to False]

### Return type

[**SettingsApiUserSettingsV1UserSettingMessage**](SettingsApiUserSettingsV1UserSettingMessage.md)

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
**200** | Success |  -  |
**404** | Not Found |  -  |
**422** | Client Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **search_my_settings**
> SettingsApiUserSettingsV1SearchUserSettingsResponse search_my_settings(application_id=application_id, setting_type_id=setting_type_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)

List User-scope settings

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.settings_api_user_settings_v1_search_user_settings_response import SettingsApiUserSettingsV1SearchUserSettingsResponse
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
    api_instance = edgraph_platform_client.MySettingsApi(api_client)
    application_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID |  (optional)
    setting_type_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID |  (optional)
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # List User-scope settings
        api_response = await api_instance.search_my_settings(application_id=application_id, setting_type_id=setting_type_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)
        print("The response of MySettingsApi->search_my_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MySettingsApi->search_my_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **application_id** | **UUID**|  | [optional] 
 **setting_type_id** | **UUID**|  | [optional] 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**SettingsApiUserSettingsV1SearchUserSettingsResponse**](SettingsApiUserSettingsV1SearchUserSettingsResponse.md)

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
**200** | Success |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **set_my_setting**
> SettingsApiUserSettingsV1SetUserSettingResponse set_my_setting(ed_graph_platform_http_aggregators_tenant_api_controllers_v1_set_my_setting_request_body=ed_graph_platform_http_aggregators_tenant_api_controllers_v1_set_my_setting_request_body)

Create or update (upsert) a User-scope setting, addressed by the SettingTypeId in the body

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_set_my_setting_request_body import EdGraphPlatformHttpAggregatorsTenantApiControllersV1SetMySettingRequestBody
from edgraph_platform_client.models.settings_api_user_settings_v1_set_user_setting_response import SettingsApiUserSettingsV1SetUserSettingResponse
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
    api_instance = edgraph_platform_client.MySettingsApi(api_client)
    ed_graph_platform_http_aggregators_tenant_api_controllers_v1_set_my_setting_request_body = edgraph_platform_client.EdGraphPlatformHttpAggregatorsTenantApiControllersV1SetMySettingRequestBody() # EdGraphPlatformHttpAggregatorsTenantApiControllersV1SetMySettingRequestBody |  (optional)

    try:
        # Create or update (upsert) a User-scope setting, addressed by the SettingTypeId in the body
        api_response = await api_instance.set_my_setting(ed_graph_platform_http_aggregators_tenant_api_controllers_v1_set_my_setting_request_body=ed_graph_platform_http_aggregators_tenant_api_controllers_v1_set_my_setting_request_body)
        print("The response of MySettingsApi->set_my_setting:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MySettingsApi->set_my_setting: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ed_graph_platform_http_aggregators_tenant_api_controllers_v1_set_my_setting_request_body** | [**EdGraphPlatformHttpAggregatorsTenantApiControllersV1SetMySettingRequestBody**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1SetMySettingRequestBody.md)|  | [optional] 

### Return type

[**SettingsApiUserSettingsV1SetUserSettingResponse**](SettingsApiUserSettingsV1SetUserSettingResponse.md)

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
**200** | Success |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_my_setting**
> update_my_setting(setting_id_or_code, ed_graph_platform_http_aggregators_tenant_api_controllers_v1_update_my_setting_request_body=ed_graph_platform_http_aggregators_tenant_api_controllers_v1_update_my_setting_request_body)

Update the User-scope setting for a key, addressed by SettingType id or Code

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_update_my_setting_request_body import EdGraphPlatformHttpAggregatorsTenantApiControllersV1UpdateMySettingRequestBody
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
    api_instance = edgraph_platform_client.MySettingsApi(api_client)
    setting_id_or_code = 'setting_id_or_code_example' # str | 
    ed_graph_platform_http_aggregators_tenant_api_controllers_v1_update_my_setting_request_body = edgraph_platform_client.EdGraphPlatformHttpAggregatorsTenantApiControllersV1UpdateMySettingRequestBody() # EdGraphPlatformHttpAggregatorsTenantApiControllersV1UpdateMySettingRequestBody |  (optional)

    try:
        # Update the User-scope setting for a key, addressed by SettingType id or Code
        await api_instance.update_my_setting(setting_id_or_code, ed_graph_platform_http_aggregators_tenant_api_controllers_v1_update_my_setting_request_body=ed_graph_platform_http_aggregators_tenant_api_controllers_v1_update_my_setting_request_body)
    except Exception as e:
        print("Exception when calling MySettingsApi->update_my_setting: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **setting_id_or_code** | **str**|  | 
 **ed_graph_platform_http_aggregators_tenant_api_controllers_v1_update_my_setting_request_body** | [**EdGraphPlatformHttpAggregatorsTenantApiControllersV1UpdateMySettingRequestBody**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1UpdateMySettingRequestBody.md)|  | [optional] 

### Return type

void (empty response body)

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
**204** | No Content |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |
**422** | Client Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

