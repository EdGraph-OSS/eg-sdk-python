# edgraph_platform_client.GroupsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_users_to_group_async**](GroupsApi.md#add_users_to_group_async) | **POST** /tenants/{tenantId}/analytics/groups/{groupId}/users/bulk | Adds users to group.
[**create_analytics_power_bi_group**](GroupsApi.md#create_analytics_power_bi_group) | **POST** /tenants/{tenantId}/analytics/groups | Creates a group.
[**delete_analytics_power_bi_group**](GroupsApi.md#delete_analytics_power_bi_group) | **DELETE** /tenants/{tenantId}/analytics/groups/{groupId} | Deletes a group.
[**get_analytics_power_bi_group_users**](GroupsApi.md#get_analytics_power_bi_group_users) | **GET** /tenants/{tenantId}/analytics/groups/{groupId}/users | Retrieves all users for a specific group.
[**get_groups_async**](GroupsApi.md#get_groups_async) | **GET** /tenants/{tenantId}/analytics/groups | Retrieves a list of groups.


# **add_users_to_group_async**
> add_users_to_group_async(tenant_id, group_id, analytics_api_groups_v1_add_group_users_request=analytics_api_groups_v1_add_group_users_request)

Adds users to group.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_groups_v1_add_group_users_request import AnalyticsApiGroupsV1AddGroupUsersRequest
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
    api_instance = edgraph_platform_client.GroupsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    group_id = 'group_id_example' # str | 
    analytics_api_groups_v1_add_group_users_request = edgraph_platform_client.AnalyticsApiGroupsV1AddGroupUsersRequest() # AnalyticsApiGroupsV1AddGroupUsersRequest |  (optional)

    try:
        # Adds users to group.
        await api_instance.add_users_to_group_async(tenant_id, group_id, analytics_api_groups_v1_add_group_users_request=analytics_api_groups_v1_add_group_users_request)
    except Exception as e:
        print("Exception when calling GroupsApi->add_users_to_group_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **group_id** | **str**|  | 
 **analytics_api_groups_v1_add_group_users_request** | [**AnalyticsApiGroupsV1AddGroupUsersRequest**](AnalyticsApiGroupsV1AddGroupUsersRequest.md)|  | [optional] 

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
**200** | The requested resource was successfully retrieved. |  -  |
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_analytics_power_bi_group**
> AnalyticsApiGroupsV1GroupResponse create_analytics_power_bi_group(tenant_id, analytics_api_groups_v1_create_group_request=analytics_api_groups_v1_create_group_request)

Creates a group.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_groups_v1_create_group_request import AnalyticsApiGroupsV1CreateGroupRequest
from edgraph_platform_client.models.analytics_api_groups_v1_group_response import AnalyticsApiGroupsV1GroupResponse
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
    api_instance = edgraph_platform_client.GroupsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    analytics_api_groups_v1_create_group_request = edgraph_platform_client.AnalyticsApiGroupsV1CreateGroupRequest() # AnalyticsApiGroupsV1CreateGroupRequest |  (optional)

    try:
        # Creates a group.
        api_response = await api_instance.create_analytics_power_bi_group(tenant_id, analytics_api_groups_v1_create_group_request=analytics_api_groups_v1_create_group_request)
        print("The response of GroupsApi->create_analytics_power_bi_group:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupsApi->create_analytics_power_bi_group: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **analytics_api_groups_v1_create_group_request** | [**AnalyticsApiGroupsV1CreateGroupRequest**](AnalyticsApiGroupsV1CreateGroupRequest.md)|  | [optional] 

### Return type

[**AnalyticsApiGroupsV1GroupResponse**](AnalyticsApiGroupsV1GroupResponse.md)

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
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_analytics_power_bi_group**
> delete_analytics_power_bi_group(tenant_id, group_id)

Deletes a group.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
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
    api_instance = edgraph_platform_client.GroupsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    group_id = 'group_id_example' # str | 

    try:
        # Deletes a group.
        await api_instance.delete_analytics_power_bi_group(tenant_id, group_id)
    except Exception as e:
        print("Exception when calling GroupsApi->delete_analytics_power_bi_group: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **group_id** | **str**|  | 

### Return type

void (empty response body)

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
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_analytics_power_bi_group_users**
> AnalyticsApiGroupsV1GroupUsersResponse get_analytics_power_bi_group_users(tenant_id, group_id, skip_first_n=skip_first_n, top_first_n=top_first_n)

Retrieves all users for a specific group.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_groups_v1_group_users_response import AnalyticsApiGroupsV1GroupUsersResponse
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
    api_instance = edgraph_platform_client.GroupsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    group_id = 'group_id_example' # str | 
    skip_first_n = 56 # int |  (optional)
    top_first_n = 56 # int |  (optional)

    try:
        # Retrieves all users for a specific group.
        api_response = await api_instance.get_analytics_power_bi_group_users(tenant_id, group_id, skip_first_n=skip_first_n, top_first_n=top_first_n)
        print("The response of GroupsApi->get_analytics_power_bi_group_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupsApi->get_analytics_power_bi_group_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **group_id** | **str**|  | 
 **skip_first_n** | **int**|  | [optional] 
 **top_first_n** | **int**|  | [optional] 

### Return type

[**AnalyticsApiGroupsV1GroupUsersResponse**](AnalyticsApiGroupsV1GroupUsersResponse.md)

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
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_groups_async**
> AnalyticsApiGroupsV1GroupsResponse get_groups_async(tenant_id, filter=filter)

Retrieves a list of groups.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_groups_v1_groups_response import AnalyticsApiGroupsV1GroupsResponse
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
    api_instance = edgraph_platform_client.GroupsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    filter = 'filter_example' # str |  (optional)

    try:
        # Retrieves a list of groups.
        api_response = await api_instance.get_groups_async(tenant_id, filter=filter)
        print("The response of GroupsApi->get_groups_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupsApi->get_groups_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **filter** | **str**|  | [optional] 

### Return type

[**AnalyticsApiGroupsV1GroupsResponse**](AnalyticsApiGroupsV1GroupsResponse.md)

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
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

