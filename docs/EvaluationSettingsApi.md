# edgraph_platform_client.EvaluationSettingsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_evaluation_setting**](EvaluationSettingsApi.md#get_evaluation_setting) | **GET** /tenants/{tenantId}/evaluations/configuration | Gets the Evaluation Settings for a given tenant
[**set_evaluation_setting_application_setting**](EvaluationSettingsApi.md#set_evaluation_setting_application_setting) | **POST** /tenants/{tenantId}/evaluations/configuration/application | Sets the Application Settings of an Evaluation for a given Tenant
[**set_evaluation_setting_user_setting**](EvaluationSettingsApi.md#set_evaluation_setting_user_setting) | **POST** /tenants/{tenantId}/evaluations/configuration/users | Sets the User Settings of an Evaluation for a given Tenant


# **get_evaluation_setting**
> EvaluationApiEvaluationSettingsV1EvaluationSettingResponse get_evaluation_setting(tenant_id)

Gets the Evaluation Settings for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.evaluation_api_evaluation_settings_v1_evaluation_setting_response import EvaluationApiEvaluationSettingsV1EvaluationSettingResponse
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
    api_instance = edgraph_platform_client.EvaluationSettingsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets the Evaluation Settings for a given tenant
        api_response = await api_instance.get_evaluation_setting(tenant_id)
        print("The response of EvaluationSettingsApi->get_evaluation_setting:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EvaluationSettingsApi->get_evaluation_setting: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 

### Return type

[**EvaluationApiEvaluationSettingsV1EvaluationSettingResponse**](EvaluationApiEvaluationSettingsV1EvaluationSettingResponse.md)

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

# **set_evaluation_setting_application_setting**
> EvaluationApiEvaluationSettingsV1ApplicationSetResponse set_evaluation_setting_application_setting(tenant_id, evaluation_api_evaluation_settings_v1_set_application_request=evaluation_api_evaluation_settings_v1_set_application_request)

Sets the Application Settings of an Evaluation for a given Tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.evaluation_api_evaluation_settings_v1_application_set_response import EvaluationApiEvaluationSettingsV1ApplicationSetResponse
from edgraph_platform_client.models.evaluation_api_evaluation_settings_v1_set_application_request import EvaluationApiEvaluationSettingsV1SetApplicationRequest
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
    api_instance = edgraph_platform_client.EvaluationSettingsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    evaluation_api_evaluation_settings_v1_set_application_request = edgraph_platform_client.EvaluationApiEvaluationSettingsV1SetApplicationRequest() # EvaluationApiEvaluationSettingsV1SetApplicationRequest |  (optional)

    try:
        # Sets the Application Settings of an Evaluation for a given Tenant
        api_response = await api_instance.set_evaluation_setting_application_setting(tenant_id, evaluation_api_evaluation_settings_v1_set_application_request=evaluation_api_evaluation_settings_v1_set_application_request)
        print("The response of EvaluationSettingsApi->set_evaluation_setting_application_setting:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EvaluationSettingsApi->set_evaluation_setting_application_setting: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **evaluation_api_evaluation_settings_v1_set_application_request** | [**EvaluationApiEvaluationSettingsV1SetApplicationRequest**](EvaluationApiEvaluationSettingsV1SetApplicationRequest.md)|  | [optional] 

### Return type

[**EvaluationApiEvaluationSettingsV1ApplicationSetResponse**](EvaluationApiEvaluationSettingsV1ApplicationSetResponse.md)

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

# **set_evaluation_setting_user_setting**
> EvaluationApiEvaluationSettingsV1UsersSetResponse set_evaluation_setting_user_setting(tenant_id, evaluation_api_evaluation_settings_v1_set_users_request=evaluation_api_evaluation_settings_v1_set_users_request)

Sets the User Settings of an Evaluation for a given Tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.evaluation_api_evaluation_settings_v1_set_users_request import EvaluationApiEvaluationSettingsV1SetUsersRequest
from edgraph_platform_client.models.evaluation_api_evaluation_settings_v1_users_set_response import EvaluationApiEvaluationSettingsV1UsersSetResponse
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
    api_instance = edgraph_platform_client.EvaluationSettingsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    evaluation_api_evaluation_settings_v1_set_users_request = edgraph_platform_client.EvaluationApiEvaluationSettingsV1SetUsersRequest() # EvaluationApiEvaluationSettingsV1SetUsersRequest |  (optional)

    try:
        # Sets the User Settings of an Evaluation for a given Tenant
        api_response = await api_instance.set_evaluation_setting_user_setting(tenant_id, evaluation_api_evaluation_settings_v1_set_users_request=evaluation_api_evaluation_settings_v1_set_users_request)
        print("The response of EvaluationSettingsApi->set_evaluation_setting_user_setting:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EvaluationSettingsApi->set_evaluation_setting_user_setting: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **evaluation_api_evaluation_settings_v1_set_users_request** | [**EvaluationApiEvaluationSettingsV1SetUsersRequest**](EvaluationApiEvaluationSettingsV1SetUsersRequest.md)|  | [optional] 

### Return type

[**EvaluationApiEvaluationSettingsV1UsersSetResponse**](EvaluationApiEvaluationSettingsV1UsersSetResponse.md)

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

