# edgraph_platform_client.InstanceResourcesCountApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_all_instance_resources_count_async**](InstanceResourcesCountApi.md#get_all_instance_resources_count_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/applications/{applicationId}/apiclients/{apiClientId}/resourcescount | Retrieves a paginated list of Instance Resources Count
[**get_all_instance_resources_count_json**](InstanceResourcesCountApi.md#get_all_instance_resources_count_json) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/applications/{applicationId}/apiclients/{apiClientId}/resourcescount/export | Retrieves the JSON representation of Instance Resources Count. Useful for exporting into other systems.


# **get_all_instance_resources_count_async**
> EdfiAdminApiEdfiAdminV1InstanceResourcesCountListResponsePaginatedItemsViewModel get_all_instance_resources_count_async(tenant_id, instance_id, year, application_id, api_client_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a paginated list of Instance Resources Count

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_resources_count_list_response_paginated_items_view_model import EdfiAdminApiEdfiAdminV1InstanceResourcesCountListResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.InstanceResourcesCountApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    application_id = 56 # int | 
    api_client_id = 56 # int | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a paginated list of Instance Resources Count
        api_response = api_instance.get_all_instance_resources_count_async(tenant_id, instance_id, year, application_id, api_client_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of InstanceResourcesCountApi->get_all_instance_resources_count_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstanceResourcesCountApi->get_all_instance_resources_count_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **application_id** | **int**|  | 
 **api_client_id** | **int**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdfiAdminApiEdfiAdminV1InstanceResourcesCountListResponsePaginatedItemsViewModel**](EdfiAdminApiEdfiAdminV1InstanceResourcesCountListResponsePaginatedItemsViewModel.md)

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

# **get_all_instance_resources_count_json**
> EdfiAdminApiEdfiAdminV1InstanceResourcesCountJsonResponse get_all_instance_resources_count_json(tenant_id, instance_id, year, application_id, api_client_id, filter=filter)

Retrieves the JSON representation of Instance Resources Count. Useful for exporting into other systems.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_resources_count_json_response import EdfiAdminApiEdfiAdminV1InstanceResourcesCountJsonResponse
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
    api_instance = edgraph_platform_client.InstanceResourcesCountApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    application_id = 56 # int | 
    api_client_id = 56 # int | 
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves the JSON representation of Instance Resources Count. Useful for exporting into other systems.
        api_response = api_instance.get_all_instance_resources_count_json(tenant_id, instance_id, year, application_id, api_client_id, filter=filter)
        print("The response of InstanceResourcesCountApi->get_all_instance_resources_count_json:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstanceResourcesCountApi->get_all_instance_resources_count_json: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **application_id** | **int**|  | 
 **api_client_id** | **int**|  | 
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdfiAdminApiEdfiAdminV1InstanceResourcesCountJsonResponse**](EdfiAdminApiEdfiAdminV1InstanceResourcesCountJsonResponse.md)

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

