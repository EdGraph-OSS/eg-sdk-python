# edgraph_platform_client.WebhooksApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_webhook_async**](WebhooksApi.md#create_webhook_async) | **POST** /tenants/{tenantId}/webhooks | Creates a new Webhook
[**delete_webhook_async**](WebhooksApi.md#delete_webhook_async) | **DELETE** /tenants/{tenantId}/webhooks/{webhookId} | Removes a webhook.
[**get_all_webhook_subscriptions_async**](WebhooksApi.md#get_all_webhook_subscriptions_async) | **GET** /tenants/{tenantId}/webhooks/events | 
[**get_all_webhooks_async**](WebhooksApi.md#get_all_webhooks_async) | **GET** /tenants/{tenantId}/webhooks | Retrieves a list of webhooks.
[**get_webhook_by_id_async**](WebhooksApi.md#get_webhook_by_id_async) | **GET** /tenants/{tenantId}/webhooks/{webhookId} | Retrieves a webhook by ID.
[**update_webhook_async**](WebhooksApi.md#update_webhook_async) | **PUT** /tenants/{tenantId}/webhooks/{webhookId} | Updates a webhook


# **create_webhook_async**
> TenantApiWebhookV1WebhookIdResponse create_webhook_async(tenant_id, tenant_api_webhook_v1_create_webhook_request=tenant_api_webhook_v1_create_webhook_request)

Creates a new Webhook

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_webhook_v1_create_webhook_request import TenantApiWebhookV1CreateWebhookRequest
from edgraph_platform_client.models.tenant_api_webhook_v1_webhook_id_response import TenantApiWebhookV1WebhookIdResponse
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
    api_instance = edgraph_platform_client.WebhooksApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    tenant_api_webhook_v1_create_webhook_request = edgraph_platform_client.TenantApiWebhookV1CreateWebhookRequest() # TenantApiWebhookV1CreateWebhookRequest |  (optional)

    try:
        # Creates a new Webhook
        api_response = api_instance.create_webhook_async(tenant_id, tenant_api_webhook_v1_create_webhook_request=tenant_api_webhook_v1_create_webhook_request)
        print("The response of WebhooksApi->create_webhook_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->create_webhook_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **tenant_api_webhook_v1_create_webhook_request** | [**TenantApiWebhookV1CreateWebhookRequest**](TenantApiWebhookV1CreateWebhookRequest.md)|  | [optional] 

### Return type

[**TenantApiWebhookV1WebhookIdResponse**](TenantApiWebhookV1WebhookIdResponse.md)

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

# **delete_webhook_async**
> TenantApiWebhookV1WebhookIdResponse delete_webhook_async(tenant_id, webhook_id)

Removes a webhook.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_webhook_v1_webhook_id_response import TenantApiWebhookV1WebhookIdResponse
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
    api_instance = edgraph_platform_client.WebhooksApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    webhook_id = 'webhook_id_example' # str | 

    try:
        # Removes a webhook.
        api_response = api_instance.delete_webhook_async(tenant_id, webhook_id)
        print("The response of WebhooksApi->delete_webhook_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->delete_webhook_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **webhook_id** | **str**|  | 

### Return type

[**TenantApiWebhookV1WebhookIdResponse**](TenantApiWebhookV1WebhookIdResponse.md)

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

# **get_all_webhook_subscriptions_async**
> TenantApiWebhookV1WebhookEventsResponse get_all_webhook_subscriptions_async(tenant_id)



### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_webhook_v1_webhook_events_response import TenantApiWebhookV1WebhookEventsResponse
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
    api_instance = edgraph_platform_client.WebhooksApi(api_client)
    tenant_id = 'tenant_id_example' # str | 

    try:
        api_response = api_instance.get_all_webhook_subscriptions_async(tenant_id)
        print("The response of WebhooksApi->get_all_webhook_subscriptions_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->get_all_webhook_subscriptions_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 

### Return type

[**TenantApiWebhookV1WebhookEventsResponse**](TenantApiWebhookV1WebhookEventsResponse.md)

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

# **get_all_webhooks_async**
> TenantApiWebhookV1PaginatedItemsResponse get_all_webhooks_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of webhooks.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_webhook_v1_paginated_items_response import TenantApiWebhookV1PaginatedItemsResponse
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
    api_instance = edgraph_platform_client.WebhooksApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of webhooks.
        api_response = api_instance.get_all_webhooks_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of WebhooksApi->get_all_webhooks_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->get_all_webhooks_async: %s\n" % e)
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

[**TenantApiWebhookV1PaginatedItemsResponse**](TenantApiWebhookV1PaginatedItemsResponse.md)

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

# **get_webhook_by_id_async**
> TenantApiWebhookV1WebhookResponse get_webhook_by_id_async(tenant_id, webhook_id)

Retrieves a webhook by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_webhook_v1_webhook_response import TenantApiWebhookV1WebhookResponse
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
    api_instance = edgraph_platform_client.WebhooksApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    webhook_id = 'webhook_id_example' # str | 

    try:
        # Retrieves a webhook by ID.
        api_response = api_instance.get_webhook_by_id_async(tenant_id, webhook_id)
        print("The response of WebhooksApi->get_webhook_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->get_webhook_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **webhook_id** | **str**|  | 

### Return type

[**TenantApiWebhookV1WebhookResponse**](TenantApiWebhookV1WebhookResponse.md)

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

# **update_webhook_async**
> TenantApiWebhookV1WebhookIdResponse update_webhook_async(tenant_id, webhook_id, tenant_api_webhook_v1_update_webhook_request=tenant_api_webhook_v1_update_webhook_request)

Updates a webhook

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_webhook_v1_update_webhook_request import TenantApiWebhookV1UpdateWebhookRequest
from edgraph_platform_client.models.tenant_api_webhook_v1_webhook_id_response import TenantApiWebhookV1WebhookIdResponse
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
    api_instance = edgraph_platform_client.WebhooksApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    webhook_id = 'webhook_id_example' # str | 
    tenant_api_webhook_v1_update_webhook_request = edgraph_platform_client.TenantApiWebhookV1UpdateWebhookRequest() # TenantApiWebhookV1UpdateWebhookRequest |  (optional)

    try:
        # Updates a webhook
        api_response = api_instance.update_webhook_async(tenant_id, webhook_id, tenant_api_webhook_v1_update_webhook_request=tenant_api_webhook_v1_update_webhook_request)
        print("The response of WebhooksApi->update_webhook_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->update_webhook_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **webhook_id** | **str**|  | 
 **tenant_api_webhook_v1_update_webhook_request** | [**TenantApiWebhookV1UpdateWebhookRequest**](TenantApiWebhookV1UpdateWebhookRequest.md)|  | [optional] 

### Return type

[**TenantApiWebhookV1WebhookIdResponse**](TenantApiWebhookV1WebhookIdResponse.md)

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

