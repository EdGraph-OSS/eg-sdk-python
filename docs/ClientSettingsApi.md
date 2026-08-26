# edgraph_platform_client.ClientSettingsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_client_setting**](ClientSettingsApi.md#create_client_setting) | **POST** /v2/tenants/{tenantId}/clients/{clientId}/settings | Create a Client-scope setting
[**delete_client_setting**](ClientSettingsApi.md#delete_client_setting) | **DELETE** /v2/tenants/{tenantId}/clients/{clientId}/settings/{settingIdOrCode} | Delete the Client-scope setting for a key, addressed by SettingType id or Code
[**get_client_setting**](ClientSettingsApi.md#get_client_setting) | **GET** /v2/tenants/{tenantId}/clients/{clientId}/settings/{settingIdOrCode} | Get a Client-scope setting
[**search_client_settings**](ClientSettingsApi.md#search_client_settings) | **GET** /v2/tenants/{tenantId}/clients/{clientId}/settings | List Client-scope settings
[**set_client_setting**](ClientSettingsApi.md#set_client_setting) | **PUT** /v2/tenants/{tenantId}/clients/{clientId}/settings | Create or update (upsert) a Client-scope setting, addressed by the SettingTypeId in the body
[**update_client_setting**](ClientSettingsApi.md#update_client_setting) | **PUT** /v2/tenants/{tenantId}/clients/{clientId}/settings/{settingIdOrCode} | Update the Client-scope setting for a key, addressed by SettingType id or Code


# **create_client_setting**
> SettingsApiClientSettingsV1CreateClientSettingResponse create_client_setting(tenant_id, client_id, ed_graph_http_aggregators_tenant_api_controllers_v2_create_client_setting_request_body=ed_graph_http_aggregators_tenant_api_controllers_v2_create_client_setting_request_body)

Create a Client-scope setting

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v2_create_client_setting_request_body import EdGraphHttpAggregatorsTenantApiControllersV2CreateClientSettingRequestBody
from edgraph_platform_client.models.settings_api_client_settings_v1_create_client_setting_response import SettingsApiClientSettingsV1CreateClientSettingResponse
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
    api_instance = edgraph_platform_client.ClientSettingsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    client_id = 'client_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v2_create_client_setting_request_body = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV2CreateClientSettingRequestBody() # EdGraphHttpAggregatorsTenantApiControllersV2CreateClientSettingRequestBody |  (optional)

    try:
        # Create a Client-scope setting
        api_response = await api_instance.create_client_setting(tenant_id, client_id, ed_graph_http_aggregators_tenant_api_controllers_v2_create_client_setting_request_body=ed_graph_http_aggregators_tenant_api_controllers_v2_create_client_setting_request_body)
        print("The response of ClientSettingsApi->create_client_setting:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ClientSettingsApi->create_client_setting: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **client_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v2_create_client_setting_request_body** | [**EdGraphHttpAggregatorsTenantApiControllersV2CreateClientSettingRequestBody**](EdGraphHttpAggregatorsTenantApiControllersV2CreateClientSettingRequestBody.md)|  | [optional] 

### Return type

[**SettingsApiClientSettingsV1CreateClientSettingResponse**](SettingsApiClientSettingsV1CreateClientSettingResponse.md)

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

# **delete_client_setting**
> delete_client_setting(tenant_id, client_id, setting_id_or_code, ed_graph_http_aggregators_tenant_api_controllers_v2_delete_client_setting_request_body=ed_graph_http_aggregators_tenant_api_controllers_v2_delete_client_setting_request_body)

Delete the Client-scope setting for a key, addressed by SettingType id or Code

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v2_delete_client_setting_request_body import EdGraphHttpAggregatorsTenantApiControllersV2DeleteClientSettingRequestBody
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
    api_instance = edgraph_platform_client.ClientSettingsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    client_id = 'client_id_example' # str | 
    setting_id_or_code = 'setting_id_or_code_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v2_delete_client_setting_request_body = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV2DeleteClientSettingRequestBody() # EdGraphHttpAggregatorsTenantApiControllersV2DeleteClientSettingRequestBody |  (optional)

    try:
        # Delete the Client-scope setting for a key, addressed by SettingType id or Code
        await api_instance.delete_client_setting(tenant_id, client_id, setting_id_or_code, ed_graph_http_aggregators_tenant_api_controllers_v2_delete_client_setting_request_body=ed_graph_http_aggregators_tenant_api_controllers_v2_delete_client_setting_request_body)
    except Exception as e:
        print("Exception when calling ClientSettingsApi->delete_client_setting: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **client_id** | **str**|  | 
 **setting_id_or_code** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v2_delete_client_setting_request_body** | [**EdGraphHttpAggregatorsTenantApiControllersV2DeleteClientSettingRequestBody**](EdGraphHttpAggregatorsTenantApiControllersV2DeleteClientSettingRequestBody.md)|  | [optional] 

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

# **get_client_setting**
> SettingsApiClientSettingsV1ClientSettingMessage get_client_setting(tenant_id, client_id, setting_id_or_code, setting_type_id=setting_type_id, provider=provider, application_id=application_id, resolve_effective_value=resolve_effective_value)

Get a Client-scope setting

Answers with the stored record alone. Effective-value resolution is opt-in: pass
`resolveEffectiveValue=true` to instead receive the value in force at this scope — every
layer above it merged under the setting's own value.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.settings_api_client_settings_v1_client_setting_message import SettingsApiClientSettingsV1ClientSettingMessage
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
    api_instance = edgraph_platform_client.ClientSettingsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    client_id = 'client_id_example' # str | 
    setting_id_or_code = 'setting_id_or_code_example' # str | 
    setting_type_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID |  (optional)
    provider = 'provider_example' # str |  (optional)
    application_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID |  (optional)
    resolve_effective_value = False # bool |  (optional) (default to False)

    try:
        # Get a Client-scope setting
        api_response = await api_instance.get_client_setting(tenant_id, client_id, setting_id_or_code, setting_type_id=setting_type_id, provider=provider, application_id=application_id, resolve_effective_value=resolve_effective_value)
        print("The response of ClientSettingsApi->get_client_setting:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ClientSettingsApi->get_client_setting: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **client_id** | **str**|  | 
 **setting_id_or_code** | **str**|  | 
 **setting_type_id** | **UUID**|  | [optional] 
 **provider** | **str**|  | [optional] 
 **application_id** | **UUID**|  | [optional] 
 **resolve_effective_value** | **bool**|  | [optional] [default to False]

### Return type

[**SettingsApiClientSettingsV1ClientSettingMessage**](SettingsApiClientSettingsV1ClientSettingMessage.md)

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

# **search_client_settings**
> SettingsApiClientSettingsV1SearchClientSettingsResponse search_client_settings(tenant_id, client_id, application_id=application_id, setting_type_id=setting_type_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)

List Client-scope settings

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.settings_api_client_settings_v1_search_client_settings_response import SettingsApiClientSettingsV1SearchClientSettingsResponse
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
    api_instance = edgraph_platform_client.ClientSettingsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    client_id = 'client_id_example' # str | 
    application_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID |  (optional)
    setting_type_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID |  (optional)
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # List Client-scope settings
        api_response = await api_instance.search_client_settings(tenant_id, client_id, application_id=application_id, setting_type_id=setting_type_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)
        print("The response of ClientSettingsApi->search_client_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ClientSettingsApi->search_client_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **client_id** | **str**|  | 
 **application_id** | **UUID**|  | [optional] 
 **setting_type_id** | **UUID**|  | [optional] 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**SettingsApiClientSettingsV1SearchClientSettingsResponse**](SettingsApiClientSettingsV1SearchClientSettingsResponse.md)

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

# **set_client_setting**
> SettingsApiClientSettingsV1SetClientSettingResponse set_client_setting(tenant_id, client_id, ed_graph_http_aggregators_tenant_api_controllers_v2_set_client_setting_request_body=ed_graph_http_aggregators_tenant_api_controllers_v2_set_client_setting_request_body)

Create or update (upsert) a Client-scope setting, addressed by the SettingTypeId in the body

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v2_set_client_setting_request_body import EdGraphHttpAggregatorsTenantApiControllersV2SetClientSettingRequestBody
from edgraph_platform_client.models.settings_api_client_settings_v1_set_client_setting_response import SettingsApiClientSettingsV1SetClientSettingResponse
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
    api_instance = edgraph_platform_client.ClientSettingsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    client_id = 'client_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v2_set_client_setting_request_body = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV2SetClientSettingRequestBody() # EdGraphHttpAggregatorsTenantApiControllersV2SetClientSettingRequestBody |  (optional)

    try:
        # Create or update (upsert) a Client-scope setting, addressed by the SettingTypeId in the body
        api_response = await api_instance.set_client_setting(tenant_id, client_id, ed_graph_http_aggregators_tenant_api_controllers_v2_set_client_setting_request_body=ed_graph_http_aggregators_tenant_api_controllers_v2_set_client_setting_request_body)
        print("The response of ClientSettingsApi->set_client_setting:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ClientSettingsApi->set_client_setting: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **client_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v2_set_client_setting_request_body** | [**EdGraphHttpAggregatorsTenantApiControllersV2SetClientSettingRequestBody**](EdGraphHttpAggregatorsTenantApiControllersV2SetClientSettingRequestBody.md)|  | [optional] 

### Return type

[**SettingsApiClientSettingsV1SetClientSettingResponse**](SettingsApiClientSettingsV1SetClientSettingResponse.md)

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

# **update_client_setting**
> update_client_setting(tenant_id, client_id, setting_id_or_code, ed_graph_http_aggregators_tenant_api_controllers_v2_update_client_setting_request_body=ed_graph_http_aggregators_tenant_api_controllers_v2_update_client_setting_request_body)

Update the Client-scope setting for a key, addressed by SettingType id or Code

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v2_update_client_setting_request_body import EdGraphHttpAggregatorsTenantApiControllersV2UpdateClientSettingRequestBody
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
    api_instance = edgraph_platform_client.ClientSettingsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    client_id = 'client_id_example' # str | 
    setting_id_or_code = 'setting_id_or_code_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v2_update_client_setting_request_body = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV2UpdateClientSettingRequestBody() # EdGraphHttpAggregatorsTenantApiControllersV2UpdateClientSettingRequestBody |  (optional)

    try:
        # Update the Client-scope setting for a key, addressed by SettingType id or Code
        await api_instance.update_client_setting(tenant_id, client_id, setting_id_or_code, ed_graph_http_aggregators_tenant_api_controllers_v2_update_client_setting_request_body=ed_graph_http_aggregators_tenant_api_controllers_v2_update_client_setting_request_body)
    except Exception as e:
        print("Exception when calling ClientSettingsApi->update_client_setting: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **client_id** | **str**|  | 
 **setting_id_or_code** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v2_update_client_setting_request_body** | [**EdGraphHttpAggregatorsTenantApiControllersV2UpdateClientSettingRequestBody**](EdGraphHttpAggregatorsTenantApiControllersV2UpdateClientSettingRequestBody.md)|  | [optional] 

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

