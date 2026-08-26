# edgraph_platform_client.MyExtensionsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**remove_user_extension**](MyExtensionsApi.md#remove_user_extension) | **DELETE** /me/extensions/{code} | Removes a user&#39;s profile extension.  &lt;br&gt;&lt;b&gt;Deprecated.&lt;/b&gt; Use &#x60;/me/settings/{code}&#x60; instead. Superseded by  EdGraph.Services.Settings; see docs/settings-deprecation-map.md. This endpoint  still works and is unchanged.
[**set_user_extension**](MyExtensionsApi.md#set_user_extension) | **POST** /me/extensions | Creates or update a user&#39;s profile extension.  &lt;br&gt;&lt;b&gt;Deprecated.&lt;/b&gt; Use &#x60;/me/settings&#x60; instead. Superseded by  EdGraph.Services.Settings; see docs/settings-deprecation-map.md. This endpoint  still works and is unchanged.


# **remove_user_extension**
> IdentityApiUserV1UserExtensionRemovedResponse remove_user_extension(code)

Removes a user's profile extension.  <br><b>Deprecated.</b> Use `/me/settings/{code}` instead. Superseded by  EdGraph.Services.Settings; see docs/settings-deprecation-map.md. This endpoint  still works and is unchanged.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v1_user_extension_removed_response import IdentityApiUserV1UserExtensionRemovedResponse
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
    api_instance = edgraph_platform_client.MyExtensionsApi(api_client)
    code = 'code_example' # str | 

    try:
        # Removes a user's profile extension.  <br><b>Deprecated.</b> Use `/me/settings/{code}` instead. Superseded by  EdGraph.Services.Settings; see docs/settings-deprecation-map.md. This endpoint  still works and is unchanged.
        api_response = await api_instance.remove_user_extension(code)
        print("The response of MyExtensionsApi->remove_user_extension:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MyExtensionsApi->remove_user_extension: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **code** | **str**|  | 

### Return type

[**IdentityApiUserV1UserExtensionRemovedResponse**](IdentityApiUserV1UserExtensionRemovedResponse.md)

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

# **set_user_extension**
> IdentityApiUserV1UserExtensionSetResponse set_user_extension(identity_api_user_v1_set_user_extension_request=identity_api_user_v1_set_user_extension_request)

Creates or update a user's profile extension.  <br><b>Deprecated.</b> Use `/me/settings` instead. Superseded by  EdGraph.Services.Settings; see docs/settings-deprecation-map.md. This endpoint  still works and is unchanged.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v1_set_user_extension_request import IdentityApiUserV1SetUserExtensionRequest
from edgraph_platform_client.models.identity_api_user_v1_user_extension_set_response import IdentityApiUserV1UserExtensionSetResponse
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
    api_instance = edgraph_platform_client.MyExtensionsApi(api_client)
    identity_api_user_v1_set_user_extension_request = edgraph_platform_client.IdentityApiUserV1SetUserExtensionRequest() # IdentityApiUserV1SetUserExtensionRequest |  (optional)

    try:
        # Creates or update a user's profile extension.  <br><b>Deprecated.</b> Use `/me/settings` instead. Superseded by  EdGraph.Services.Settings; see docs/settings-deprecation-map.md. This endpoint  still works and is unchanged.
        api_response = await api_instance.set_user_extension(identity_api_user_v1_set_user_extension_request=identity_api_user_v1_set_user_extension_request)
        print("The response of MyExtensionsApi->set_user_extension:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MyExtensionsApi->set_user_extension: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **identity_api_user_v1_set_user_extension_request** | [**IdentityApiUserV1SetUserExtensionRequest**](IdentityApiUserV1SetUserExtensionRequest.md)|  | [optional] 

### Return type

[**IdentityApiUserV1UserExtensionSetResponse**](IdentityApiUserV1UserExtensionSetResponse.md)

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

