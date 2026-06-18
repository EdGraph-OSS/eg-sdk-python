# edgraph_platform_client.IntegrationProductsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_integration_product**](IntegrationProductsApi.md#create_integration_product) | **POST** /integrations/products | Creates an Integration Product.
[**delete_integration_product**](IntegrationProductsApi.md#delete_integration_product) | **DELETE** /integrations/products/{productId} | Removes an Integration Product.
[**get_integration_product**](IntegrationProductsApi.md#get_integration_product) | **GET** /integrations/products/{productId} | Gets an Integration Product.
[**search_integration_products**](IntegrationProductsApi.md#search_integration_products) | **GET** /integrations/products | Search Integration Products.
[**update_integration_product**](IntegrationProductsApi.md#update_integration_product) | **PUT** /integrations/products/{productId} | Updates an Integration Product.


# **create_integration_product**
> TenantApiIntegrationsV1CreateIntegrationProductResponse create_integration_product(tenant_api_integrations_v1_create_integration_product_request=tenant_api_integrations_v1_create_integration_product_request)

Creates an Integration Product.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_create_integration_product_request import TenantApiIntegrationsV1CreateIntegrationProductRequest
from edgraph_platform_client.models.tenant_api_integrations_v1_create_integration_product_response import TenantApiIntegrationsV1CreateIntegrationProductResponse
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
    api_instance = edgraph_platform_client.IntegrationProductsApi(api_client)
    tenant_api_integrations_v1_create_integration_product_request = edgraph_platform_client.TenantApiIntegrationsV1CreateIntegrationProductRequest() # TenantApiIntegrationsV1CreateIntegrationProductRequest |  (optional)

    try:
        # Creates an Integration Product.
        api_response = await api_instance.create_integration_product(tenant_api_integrations_v1_create_integration_product_request=tenant_api_integrations_v1_create_integration_product_request)
        print("The response of IntegrationProductsApi->create_integration_product:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationProductsApi->create_integration_product: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_api_integrations_v1_create_integration_product_request** | [**TenantApiIntegrationsV1CreateIntegrationProductRequest**](TenantApiIntegrationsV1CreateIntegrationProductRequest.md)|  | [optional] 

### Return type

[**TenantApiIntegrationsV1CreateIntegrationProductResponse**](TenantApiIntegrationsV1CreateIntegrationProductResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_integration_product**
> TenantApiIntegrationsV1DeleteIntegrationProductResponse delete_integration_product(product_id)

Removes an Integration Product.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_delete_integration_product_response import TenantApiIntegrationsV1DeleteIntegrationProductResponse
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
    api_instance = edgraph_platform_client.IntegrationProductsApi(api_client)
    product_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Removes an Integration Product.
        api_response = await api_instance.delete_integration_product(product_id)
        print("The response of IntegrationProductsApi->delete_integration_product:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationProductsApi->delete_integration_product: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **product_id** | **UUID**|  | 

### Return type

[**TenantApiIntegrationsV1DeleteIntegrationProductResponse**](TenantApiIntegrationsV1DeleteIntegrationProductResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_integration_product**
> TenantApiIntegrationsV1GetIntegrationProductResponse get_integration_product(product_id)

Gets an Integration Product.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_get_integration_product_response import TenantApiIntegrationsV1GetIntegrationProductResponse
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
    api_instance = edgraph_platform_client.IntegrationProductsApi(api_client)
    product_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets an Integration Product.
        api_response = await api_instance.get_integration_product(product_id)
        print("The response of IntegrationProductsApi->get_integration_product:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationProductsApi->get_integration_product: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **product_id** | **UUID**|  | 

### Return type

[**TenantApiIntegrationsV1GetIntegrationProductResponse**](TenantApiIntegrationsV1GetIntegrationProductResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **search_integration_products**
> TenantApiIntegrationsV1IntegrationProductPaginatedItemsViewModel search_integration_products(page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Search Integration Products.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_integration_product_paginated_items_view_model import TenantApiIntegrationsV1IntegrationProductPaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.IntegrationProductsApi(api_client)
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Search Integration Products.
        api_response = await api_instance.search_integration_products(page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of IntegrationProductsApi->search_integration_products:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationProductsApi->search_integration_products: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**TenantApiIntegrationsV1IntegrationProductPaginatedItemsViewModel**](TenantApiIntegrationsV1IntegrationProductPaginatedItemsViewModel.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_integration_product**
> object update_integration_product(product_id, tenant_api_integrations_v1_update_integration_product_request=tenant_api_integrations_v1_update_integration_product_request)

Updates an Integration Product.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_integrations_v1_update_integration_product_request import TenantApiIntegrationsV1UpdateIntegrationProductRequest
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
    api_instance = edgraph_platform_client.IntegrationProductsApi(api_client)
    product_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    tenant_api_integrations_v1_update_integration_product_request = edgraph_platform_client.TenantApiIntegrationsV1UpdateIntegrationProductRequest() # TenantApiIntegrationsV1UpdateIntegrationProductRequest |  (optional)

    try:
        # Updates an Integration Product.
        api_response = await api_instance.update_integration_product(product_id, tenant_api_integrations_v1_update_integration_product_request=tenant_api_integrations_v1_update_integration_product_request)
        print("The response of IntegrationProductsApi->update_integration_product:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationProductsApi->update_integration_product: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **product_id** | **UUID**|  | 
 **tenant_api_integrations_v1_update_integration_product_request** | [**TenantApiIntegrationsV1UpdateIntegrationProductRequest**](TenantApiIntegrationsV1UpdateIntegrationProductRequest.md)|  | [optional] 

### Return type

**object**

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

