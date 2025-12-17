# edgraph_platform_client.UsersSEOAAsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_user_seoaa**](UsersSEOAAsApi.md#add_user_seoaa) | **POST** /v2/tenants/{tenantId}/users/{userId}/seoaas | Add User SEOAAs
[**delete_user_seoaa**](UsersSEOAAsApi.md#delete_user_seoaa) | **DELETE** /v2/tenants/{tenantId}/users/{userId}/seoaas/{seoaaId} | Delete User SEOAAs
[**search_user_seoaa**](UsersSEOAAsApi.md#search_user_seoaa) | **GET** /v2/tenants/{tenantId}/users/{userId}/seoaas | Search User SEOAAs
[**update_user_seoaa**](UsersSEOAAsApi.md#update_user_seoaa) | **PUT** /v2/tenants/{tenantId}/users/{userId}/seoaas/{seoaaId} | Update User SEOAAs


# **add_user_seoaa**
> IdentityApiUserV1SEOAAAddedResponse add_user_seoaa(tenant_id, user_id, ed_graph_http_aggregators_tenant_api_controllers_v2_requests_add_seoaa_request=ed_graph_http_aggregators_tenant_api_controllers_v2_requests_add_seoaa_request)

Add User SEOAAs

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v2_requests_add_seoaa_request import EdGraphHttpAggregatorsTenantApiControllersV2RequestsAddSeoaaRequest
from edgraph_platform_client.models.identity_api_user_v1_seoaa_added_response import IdentityApiUserV1SEOAAAddedResponse
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
    api_instance = edgraph_platform_client.UsersSEOAAsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    user_id = 'user_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v2_requests_add_seoaa_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV2RequestsAddSeoaaRequest() # EdGraphHttpAggregatorsTenantApiControllersV2RequestsAddSeoaaRequest |  (optional)

    try:
        # Add User SEOAAs
        api_response = api_instance.add_user_seoaa(tenant_id, user_id, ed_graph_http_aggregators_tenant_api_controllers_v2_requests_add_seoaa_request=ed_graph_http_aggregators_tenant_api_controllers_v2_requests_add_seoaa_request)
        print("The response of UsersSEOAAsApi->add_user_seoaa:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersSEOAAsApi->add_user_seoaa: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **user_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v2_requests_add_seoaa_request** | [**EdGraphHttpAggregatorsTenantApiControllersV2RequestsAddSeoaaRequest**](EdGraphHttpAggregatorsTenantApiControllersV2RequestsAddSeoaaRequest.md)|  | [optional] 

### Return type

[**IdentityApiUserV1SEOAAAddedResponse**](IdentityApiUserV1SEOAAAddedResponse.md)

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

# **delete_user_seoaa**
> IdentityApiUserV1SEOAAUpdatedResponse delete_user_seoaa(tenant_id, user_id, seoaa_id)

Delete User SEOAAs

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v1_seoaa_updated_response import IdentityApiUserV1SEOAAUpdatedResponse
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
    api_instance = edgraph_platform_client.UsersSEOAAsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    user_id = 'user_id_example' # str | 
    seoaa_id = 'seoaa_id_example' # str | 

    try:
        # Delete User SEOAAs
        api_response = api_instance.delete_user_seoaa(tenant_id, user_id, seoaa_id)
        print("The response of UsersSEOAAsApi->delete_user_seoaa:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersSEOAAsApi->delete_user_seoaa: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **user_id** | **str**|  | 
 **seoaa_id** | **str**|  | 

### Return type

[**IdentityApiUserV1SEOAAUpdatedResponse**](IdentityApiUserV1SEOAAUpdatedResponse.md)

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

# **search_user_seoaa**
> IdentityApiUserV1GetSEOAAsResponse search_user_seoaa(tenant_id, user_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Search User SEOAAs

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v1_get_seoaas_response import IdentityApiUserV1GetSEOAAsResponse
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
    api_instance = edgraph_platform_client.UsersSEOAAsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    user_id = 'user_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Search User SEOAAs
        api_response = api_instance.search_user_seoaa(tenant_id, user_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of UsersSEOAAsApi->search_user_seoaa:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersSEOAAsApi->search_user_seoaa: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **user_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**IdentityApiUserV1GetSEOAAsResponse**](IdentityApiUserV1GetSEOAAsResponse.md)

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

# **update_user_seoaa**
> IdentityApiUserV1SEOAAUpdatedResponse update_user_seoaa(tenant_id, user_id, seoaa_id, ed_graph_http_aggregators_tenant_api_controllers_v2_requests_update_seoaa_request=ed_graph_http_aggregators_tenant_api_controllers_v2_requests_update_seoaa_request)

Update User SEOAAs

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v2_requests_update_seoaa_request import EdGraphHttpAggregatorsTenantApiControllersV2RequestsUpdateSeoaaRequest
from edgraph_platform_client.models.identity_api_user_v1_seoaa_updated_response import IdentityApiUserV1SEOAAUpdatedResponse
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
    api_instance = edgraph_platform_client.UsersSEOAAsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    user_id = 'user_id_example' # str | 
    seoaa_id = 'seoaa_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v2_requests_update_seoaa_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV2RequestsUpdateSeoaaRequest() # EdGraphHttpAggregatorsTenantApiControllersV2RequestsUpdateSeoaaRequest |  (optional)

    try:
        # Update User SEOAAs
        api_response = api_instance.update_user_seoaa(tenant_id, user_id, seoaa_id, ed_graph_http_aggregators_tenant_api_controllers_v2_requests_update_seoaa_request=ed_graph_http_aggregators_tenant_api_controllers_v2_requests_update_seoaa_request)
        print("The response of UsersSEOAAsApi->update_user_seoaa:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersSEOAAsApi->update_user_seoaa: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **user_id** | **str**|  | 
 **seoaa_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v2_requests_update_seoaa_request** | [**EdGraphHttpAggregatorsTenantApiControllersV2RequestsUpdateSeoaaRequest**](EdGraphHttpAggregatorsTenantApiControllersV2RequestsUpdateSeoaaRequest.md)|  | [optional] 

### Return type

[**IdentityApiUserV1SEOAAUpdatedResponse**](IdentityApiUserV1SEOAAUpdatedResponse.md)

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

