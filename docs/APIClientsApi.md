# edgraph_platform_client.APIClientsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_tenant_api_client_async**](APIClientsApi.md#create_tenant_api_client_async) | **POST** /tenants/{tenantId}/apiclients | Creates a new OpenId API Client
[**delete_tenant_api_client_async**](APIClientsApi.md#delete_tenant_api_client_async) | **DELETE** /tenants/{tenantId}/apiclients/{clientId} | Deletes an OpenId API Client
[**get_all_tenant_api_clients_async**](APIClientsApi.md#get_all_tenant_api_clients_async) | **GET** /tenants/{tenantId}/apiclients | Retrieves a list of OpenId API Clients associated to this tenant
[**get_tenant_api_client_by_id_async**](APIClientsApi.md#get_tenant_api_client_by_id_async) | **GET** /tenants/{tenantId}/apiclients/{clientId} | Retrieves an OpenId API Client
[**regenerate_tenant_api_client_secret_async**](APIClientsApi.md#regenerate_tenant_api_client_secret_async) | **PUT** /tenants/{tenantId}/apiclients/{clientId}/regeneratesecret | Regenerates an OpenId API Client&#39;s secret
[**update_tenant_api_client_async**](APIClientsApi.md#update_tenant_api_client_async) | **PUT** /tenants/{tenantId}/apiclients/{clientId} | Updates an OpenId API Client


# **create_tenant_api_client_async**
> IdentityApiApiClientV1ApiClientCreatedResponse create_tenant_api_client_async(tenant_id, identity_api_api_client_v1_create_api_client_request=identity_api_api_client_v1_create_api_client_request)

Creates a new OpenId API Client

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_api_client_v1_api_client_created_response import IdentityApiApiClientV1ApiClientCreatedResponse
from edgraph_platform_client.models.identity_api_api_client_v1_create_api_client_request import IdentityApiApiClientV1CreateApiClientRequest
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
    api_instance = edgraph_platform_client.APIClientsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    identity_api_api_client_v1_create_api_client_request = edgraph_platform_client.IdentityApiApiClientV1CreateApiClientRequest() # IdentityApiApiClientV1CreateApiClientRequest |  (optional)

    try:
        # Creates a new OpenId API Client
        api_response = await api_instance.create_tenant_api_client_async(tenant_id, identity_api_api_client_v1_create_api_client_request=identity_api_api_client_v1_create_api_client_request)
        print("The response of APIClientsApi->create_tenant_api_client_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling APIClientsApi->create_tenant_api_client_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **identity_api_api_client_v1_create_api_client_request** | [**IdentityApiApiClientV1CreateApiClientRequest**](IdentityApiApiClientV1CreateApiClientRequest.md)|  | [optional] 

### Return type

[**IdentityApiApiClientV1ApiClientCreatedResponse**](IdentityApiApiClientV1ApiClientCreatedResponse.md)

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

# **delete_tenant_api_client_async**
> delete_tenant_api_client_async(tenant_id, client_id)

Deletes an OpenId API Client

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
    api_instance = edgraph_platform_client.APIClientsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    client_id = 'client_id_example' # str | 

    try:
        # Deletes an OpenId API Client
        await api_instance.delete_tenant_api_client_async(tenant_id, client_id)
    except Exception as e:
        print("Exception when calling APIClientsApi->delete_tenant_api_client_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **client_id** | **str**|  | 

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
**204** | The resource was successfully deleted. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_all_tenant_api_clients_async**
> IdentityApiApiClientV1ApiClientPaginatedItemsResponsePaginatedItemsViewModel get_all_tenant_api_clients_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of OpenId API Clients associated to this tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_api_client_v1_api_client_paginated_items_response_paginated_items_view_model import IdentityApiApiClientV1ApiClientPaginatedItemsResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.APIClientsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of OpenId API Clients associated to this tenant
        api_response = await api_instance.get_all_tenant_api_clients_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of APIClientsApi->get_all_tenant_api_clients_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling APIClientsApi->get_all_tenant_api_clients_async: %s\n" % e)
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

[**IdentityApiApiClientV1ApiClientPaginatedItemsResponsePaginatedItemsViewModel**](IdentityApiApiClientV1ApiClientPaginatedItemsResponsePaginatedItemsViewModel.md)

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

# **get_tenant_api_client_by_id_async**
> IdentityApiApiClientV1ApiClientProfileResponse get_tenant_api_client_by_id_async(tenant_id, client_id)

Retrieves an OpenId API Client

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_api_client_v1_api_client_profile_response import IdentityApiApiClientV1ApiClientProfileResponse
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
    api_instance = edgraph_platform_client.APIClientsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    client_id = 'client_id_example' # str | 

    try:
        # Retrieves an OpenId API Client
        api_response = await api_instance.get_tenant_api_client_by_id_async(tenant_id, client_id)
        print("The response of APIClientsApi->get_tenant_api_client_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling APIClientsApi->get_tenant_api_client_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **client_id** | **str**|  | 

### Return type

[**IdentityApiApiClientV1ApiClientProfileResponse**](IdentityApiApiClientV1ApiClientProfileResponse.md)

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

# **regenerate_tenant_api_client_secret_async**
> IdentityApiApiClientV1ApiClientSecretRegeneratedResponse regenerate_tenant_api_client_secret_async(tenant_id, client_id, identity_api_api_client_v1_regenerate_api_client_secret_request=identity_api_api_client_v1_regenerate_api_client_secret_request)

Regenerates an OpenId API Client's secret

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_api_client_v1_api_client_secret_regenerated_response import IdentityApiApiClientV1ApiClientSecretRegeneratedResponse
from edgraph_platform_client.models.identity_api_api_client_v1_regenerate_api_client_secret_request import IdentityApiApiClientV1RegenerateApiClientSecretRequest
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
    api_instance = edgraph_platform_client.APIClientsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    client_id = 'client_id_example' # str | 
    identity_api_api_client_v1_regenerate_api_client_secret_request = edgraph_platform_client.IdentityApiApiClientV1RegenerateApiClientSecretRequest() # IdentityApiApiClientV1RegenerateApiClientSecretRequest |  (optional)

    try:
        # Regenerates an OpenId API Client's secret
        api_response = await api_instance.regenerate_tenant_api_client_secret_async(tenant_id, client_id, identity_api_api_client_v1_regenerate_api_client_secret_request=identity_api_api_client_v1_regenerate_api_client_secret_request)
        print("The response of APIClientsApi->regenerate_tenant_api_client_secret_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling APIClientsApi->regenerate_tenant_api_client_secret_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **client_id** | **str**|  | 
 **identity_api_api_client_v1_regenerate_api_client_secret_request** | [**IdentityApiApiClientV1RegenerateApiClientSecretRequest**](IdentityApiApiClientV1RegenerateApiClientSecretRequest.md)|  | [optional] 

### Return type

[**IdentityApiApiClientV1ApiClientSecretRegeneratedResponse**](IdentityApiApiClientV1ApiClientSecretRegeneratedResponse.md)

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

# **update_tenant_api_client_async**
> IdentityApiApiClientV1ApiClientUpdatedResponse update_tenant_api_client_async(tenant_id, client_id, identity_api_api_client_v1_update_api_client_request=identity_api_api_client_v1_update_api_client_request)

Updates an OpenId API Client

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_api_client_v1_api_client_updated_response import IdentityApiApiClientV1ApiClientUpdatedResponse
from edgraph_platform_client.models.identity_api_api_client_v1_update_api_client_request import IdentityApiApiClientV1UpdateApiClientRequest
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
    api_instance = edgraph_platform_client.APIClientsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    client_id = 'client_id_example' # str | 
    identity_api_api_client_v1_update_api_client_request = edgraph_platform_client.IdentityApiApiClientV1UpdateApiClientRequest() # IdentityApiApiClientV1UpdateApiClientRequest |  (optional)

    try:
        # Updates an OpenId API Client
        api_response = await api_instance.update_tenant_api_client_async(tenant_id, client_id, identity_api_api_client_v1_update_api_client_request=identity_api_api_client_v1_update_api_client_request)
        print("The response of APIClientsApi->update_tenant_api_client_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling APIClientsApi->update_tenant_api_client_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **client_id** | **str**|  | 
 **identity_api_api_client_v1_update_api_client_request** | [**IdentityApiApiClientV1UpdateApiClientRequest**](IdentityApiApiClientV1UpdateApiClientRequest.md)|  | [optional] 

### Return type

[**IdentityApiApiClientV1ApiClientUpdatedResponse**](IdentityApiApiClientV1ApiClientUpdatedResponse.md)

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

