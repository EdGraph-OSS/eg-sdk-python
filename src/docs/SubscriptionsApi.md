# edgraph_platform_client.SubscriptionsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_tenant_subscription_async**](SubscriptionsApi.md#create_tenant_subscription_async) | **POST** /tenants/{tenantId}/subscriptions | Creates a new subscription
[**get_all_tenant_subscription_applications**](SubscriptionsApi.md#get_all_tenant_subscription_applications) | **GET** /tenants/{tenantId}/subscriptions/applications | Retrieves a list of applications available for subscription.
[**get_all_tenant_subscriptions_async**](SubscriptionsApi.md#get_all_tenant_subscriptions_async) | **GET** /tenants/{tenantId}/subscriptions | Retrieves a list of subscriptions associated to this tenant
[**get_tenant_subscription_profile_by_id_async**](SubscriptionsApi.md#get_tenant_subscription_profile_by_id_async) | **GET** /tenants/{tenantId}/subscriptions/{subscriptionId} | Retrieves a subscription
[**update_tenant_subscription_async**](SubscriptionsApi.md#update_tenant_subscription_async) | **PUT** /tenants/{tenantId}/subscriptions/{subscriptionId} | Updates a subscription


# **create_tenant_subscription_async**
> TenantApiTenantV1SubscriptionCreatedResponse create_tenant_subscription_async(tenant_id, tenant_api_tenant_v1_create_subscription_request=tenant_api_tenant_v1_create_subscription_request)

Creates a new subscription

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_tenant_v1_create_subscription_request import TenantApiTenantV1CreateSubscriptionRequest
from edgraph_platform_client.models.tenant_api_tenant_v1_subscription_created_response import TenantApiTenantV1SubscriptionCreatedResponse
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
    api_instance = edgraph_platform_client.SubscriptionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    tenant_api_tenant_v1_create_subscription_request = edgraph_platform_client.TenantApiTenantV1CreateSubscriptionRequest() # TenantApiTenantV1CreateSubscriptionRequest |  (optional)

    try:
        # Creates a new subscription
        api_response = api_instance.create_tenant_subscription_async(tenant_id, tenant_api_tenant_v1_create_subscription_request=tenant_api_tenant_v1_create_subscription_request)
        print("The response of SubscriptionsApi->create_tenant_subscription_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->create_tenant_subscription_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **tenant_api_tenant_v1_create_subscription_request** | [**TenantApiTenantV1CreateSubscriptionRequest**](TenantApiTenantV1CreateSubscriptionRequest.md)|  | [optional] 

### Return type

[**TenantApiTenantV1SubscriptionCreatedResponse**](TenantApiTenantV1SubscriptionCreatedResponse.md)

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
**201** | The resource was created. The location of the resource is available in the Location header of the response. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_all_tenant_subscription_applications**
> ApplicationApiApplicationV1PaginatedItemsResponse get_all_tenant_subscription_applications(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by)

Retrieves a list of applications available for subscription.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.application_api_application_v1_paginated_items_response import ApplicationApiApplicationV1PaginatedItemsResponse
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
    api_instance = edgraph_platform_client.SubscriptionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = 'order_by_example' # str |  (optional)

    try:
        # Retrieves a list of applications available for subscription.
        api_response = api_instance.get_all_tenant_subscription_applications(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by)
        print("The response of SubscriptionsApi->get_all_tenant_subscription_applications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->get_all_tenant_subscription_applications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **order_by** | **str**|  | [optional] 

### Return type

[**ApplicationApiApplicationV1PaginatedItemsResponse**](ApplicationApiApplicationV1PaginatedItemsResponse.md)

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

# **get_all_tenant_subscriptions_async**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesSubscriptionListResponseDtoPaginatedItemsViewModel get_all_tenant_subscriptions_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of subscriptions associated to this tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_subscription_list_response_dto_paginated_items_view_model import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesSubscriptionListResponseDtoPaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.SubscriptionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of subscriptions associated to this tenant
        api_response = api_instance.get_all_tenant_subscriptions_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of SubscriptionsApi->get_all_tenant_subscriptions_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->get_all_tenant_subscriptions_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesSubscriptionListResponseDtoPaginatedItemsViewModel**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesSubscriptionListResponseDtoPaginatedItemsViewModel.md)

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

# **get_tenant_subscription_profile_by_id_async**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesSubscriptionProfileResponseDto get_tenant_subscription_profile_by_id_async(tenant_id, subscription_id)

Retrieves a subscription

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_subscription_profile_response_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesSubscriptionProfileResponseDto
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
    api_instance = edgraph_platform_client.SubscriptionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    subscription_id = 'subscription_id_example' # str | 

    try:
        # Retrieves a subscription
        api_response = api_instance.get_tenant_subscription_profile_by_id_async(tenant_id, subscription_id)
        print("The response of SubscriptionsApi->get_tenant_subscription_profile_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->get_tenant_subscription_profile_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **subscription_id** | **str**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesSubscriptionProfileResponseDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesSubscriptionProfileResponseDto.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_tenant_subscription_async**
> TenantApiTenantV1SubscriptionUpdatedResponse update_tenant_subscription_async(tenant_id, subscription_id, tenant_api_tenant_v1_update_subscription_request=tenant_api_tenant_v1_update_subscription_request)

Updates a subscription

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_tenant_v1_subscription_updated_response import TenantApiTenantV1SubscriptionUpdatedResponse
from edgraph_platform_client.models.tenant_api_tenant_v1_update_subscription_request import TenantApiTenantV1UpdateSubscriptionRequest
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
    api_instance = edgraph_platform_client.SubscriptionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    subscription_id = 'subscription_id_example' # str | 
    tenant_api_tenant_v1_update_subscription_request = edgraph_platform_client.TenantApiTenantV1UpdateSubscriptionRequest() # TenantApiTenantV1UpdateSubscriptionRequest |  (optional)

    try:
        # Updates a subscription
        api_response = api_instance.update_tenant_subscription_async(tenant_id, subscription_id, tenant_api_tenant_v1_update_subscription_request=tenant_api_tenant_v1_update_subscription_request)
        print("The response of SubscriptionsApi->update_tenant_subscription_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->update_tenant_subscription_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **subscription_id** | **str**|  | 
 **tenant_api_tenant_v1_update_subscription_request** | [**TenantApiTenantV1UpdateSubscriptionRequest**](TenantApiTenantV1UpdateSubscriptionRequest.md)|  | [optional] 

### Return type

[**TenantApiTenantV1SubscriptionUpdatedResponse**](TenantApiTenantV1SubscriptionUpdatedResponse.md)

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

