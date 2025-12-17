# edgraph_platform_client.ProvidersApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_all_tenant_data_sync_providers**](ProvidersApi.md#get_all_tenant_data_sync_providers) | **GET** /tenants/{tenantId}/datasync/providers | Retrieves a list of DataSync providers
[**get_tenant_data_sync_provider_profile_by_id**](ProvidersApi.md#get_tenant_data_sync_provider_profile_by_id) | **GET** /tenants/{tenantId}/datasync/providers/{providerId} | Retrieves a specific DataSync provider using its primary key


# **get_all_tenant_data_sync_providers**
> DataSyncApiProviderV1ProviderListResponsePaginatedItemsViewModel get_all_tenant_data_sync_providers(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of DataSync providers

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_provider_v1_provider_list_response_paginated_items_view_model import DataSyncApiProviderV1ProviderListResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.ProvidersApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of DataSync providers
        api_response = api_instance.get_all_tenant_data_sync_providers(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of ProvidersApi->get_all_tenant_data_sync_providers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProvidersApi->get_all_tenant_data_sync_providers: %s\n" % e)
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

[**DataSyncApiProviderV1ProviderListResponsePaginatedItemsViewModel**](DataSyncApiProviderV1ProviderListResponsePaginatedItemsViewModel.md)

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

# **get_tenant_data_sync_provider_profile_by_id**
> DataSyncApiProviderV1ProviderProfileResponse get_tenant_data_sync_provider_profile_by_id(tenant_id, provider_id)

Retrieves a specific DataSync provider using its primary key

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_provider_v1_provider_profile_response import DataSyncApiProviderV1ProviderProfileResponse
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
    api_instance = edgraph_platform_client.ProvidersApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    provider_id = 'provider_id_example' # str | 

    try:
        # Retrieves a specific DataSync provider using its primary key
        api_response = api_instance.get_tenant_data_sync_provider_profile_by_id(tenant_id, provider_id)
        print("The response of ProvidersApi->get_tenant_data_sync_provider_profile_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProvidersApi->get_tenant_data_sync_provider_profile_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **provider_id** | **str**|  | 

### Return type

[**DataSyncApiProviderV1ProviderProfileResponse**](DataSyncApiProviderV1ProviderProfileResponse.md)

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

