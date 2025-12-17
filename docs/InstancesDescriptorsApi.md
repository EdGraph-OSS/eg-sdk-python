# edgraph_platform_client.InstancesDescriptorsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_descriptor_async**](InstancesDescriptorsApi.md#create_descriptor_async) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/descriptors | Creates a Descriptor.
[**delete_descriptor_async**](InstancesDescriptorsApi.md#delete_descriptor_async) | **DELETE** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/descriptors/{descriptorId} | Deletes a Descriptor.
[**get_descriptor_by_id_async**](InstancesDescriptorsApi.md#get_descriptor_by_id_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/descriptors/{descriptorId} | Retrieves a Descriptor by ID.
[**get_descriptor_namespaces_async**](InstancesDescriptorsApi.md#get_descriptor_namespaces_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/namespaces | Retrieves a list of Descriptor Namespaces.
[**get_descriptors_async**](InstancesDescriptorsApi.md#get_descriptors_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/descriptors | Retrieves a list of Descriptors.
[**update_descriptor_async**](InstancesDescriptorsApi.md#update_descriptor_async) | **PUT** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/descriptors/{descriptorId} | Updates a Descriptor.


# **create_descriptor_async**
> EdfiAdminApiEdfiAdminV1DescriptorCreatedResponse create_descriptor_async(tenant_id, instance_id, year, edfi_admin_api_edfi_admin_v1_descriptor_type=edfi_admin_api_edfi_admin_v1_descriptor_type)

Creates a Descriptor.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_descriptor_created_response import EdfiAdminApiEdfiAdminV1DescriptorCreatedResponse
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_descriptor_type import EdfiAdminApiEdfiAdminV1DescriptorType
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
    api_instance = edgraph_platform_client.InstancesDescriptorsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    edfi_admin_api_edfi_admin_v1_descriptor_type = edgraph_platform_client.EdfiAdminApiEdfiAdminV1DescriptorType() # EdfiAdminApiEdfiAdminV1DescriptorType |  (optional)

    try:
        # Creates a Descriptor.
        api_response = api_instance.create_descriptor_async(tenant_id, instance_id, year, edfi_admin_api_edfi_admin_v1_descriptor_type=edfi_admin_api_edfi_admin_v1_descriptor_type)
        print("The response of InstancesDescriptorsApi->create_descriptor_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesDescriptorsApi->create_descriptor_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **edfi_admin_api_edfi_admin_v1_descriptor_type** | [**EdfiAdminApiEdfiAdminV1DescriptorType**](EdfiAdminApiEdfiAdminV1DescriptorType.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1DescriptorCreatedResponse**](EdfiAdminApiEdfiAdminV1DescriptorCreatedResponse.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_descriptor_async**
> delete_descriptor_async(tenant_id, instance_id, year, descriptor_id)

Deletes a Descriptor.

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
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.InstancesDescriptorsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    descriptor_id = 56 # int | 

    try:
        # Deletes a Descriptor.
        api_instance.delete_descriptor_async(tenant_id, instance_id, year, descriptor_id)
    except Exception as e:
        print("Exception when calling InstancesDescriptorsApi->delete_descriptor_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **descriptor_id** | **int**|  | 

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_descriptor_by_id_async**
> EdfiAdminApiEdfiAdminV1DescriptorType get_descriptor_by_id_async(tenant_id, instance_id, year, descriptor_id)

Retrieves a Descriptor by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_descriptor_type import EdfiAdminApiEdfiAdminV1DescriptorType
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
    api_instance = edgraph_platform_client.InstancesDescriptorsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    descriptor_id = 56 # int | 

    try:
        # Retrieves a Descriptor by ID.
        api_response = api_instance.get_descriptor_by_id_async(tenant_id, instance_id, year, descriptor_id)
        print("The response of InstancesDescriptorsApi->get_descriptor_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesDescriptorsApi->get_descriptor_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **descriptor_id** | **int**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1DescriptorType**](EdfiAdminApiEdfiAdminV1DescriptorType.md)

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

# **get_descriptor_namespaces_async**
> EdfiAdminApiEdfiAdminV1DescriptorNamespacesPaginatedItemsResponse get_descriptor_namespaces_async(tenant_id, instance_id, year, page_size=page_size, page_index=page_index)

Retrieves a list of Descriptor Namespaces.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_descriptor_namespaces_paginated_items_response import EdfiAdminApiEdfiAdminV1DescriptorNamespacesPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.InstancesDescriptorsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)

    try:
        # Retrieves a list of Descriptor Namespaces.
        api_response = api_instance.get_descriptor_namespaces_async(tenant_id, instance_id, year, page_size=page_size, page_index=page_index)
        print("The response of InstancesDescriptorsApi->get_descriptor_namespaces_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesDescriptorsApi->get_descriptor_namespaces_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]

### Return type

[**EdfiAdminApiEdfiAdminV1DescriptorNamespacesPaginatedItemsResponse**](EdfiAdminApiEdfiAdminV1DescriptorNamespacesPaginatedItemsResponse.md)

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

# **get_descriptors_async**
> EdfiAdminApiEdfiAdminV1DescriptorsPaginatedItemsResponse get_descriptors_async(tenant_id, instance_id, year, page_size=page_size, page_index=page_index, filter=filter, order_by=order_by)

Retrieves a list of Descriptors.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_descriptors_paginated_items_response import EdfiAdminApiEdfiAdminV1DescriptorsPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.InstancesDescriptorsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    filter = 'filter_example' # str |  (optional)
    order_by = 'order_by_example' # str |  (optional)

    try:
        # Retrieves a list of Descriptors.
        api_response = api_instance.get_descriptors_async(tenant_id, instance_id, year, page_size=page_size, page_index=page_index, filter=filter, order_by=order_by)
        print("The response of InstancesDescriptorsApi->get_descriptors_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesDescriptorsApi->get_descriptors_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **filter** | **str**|  | [optional] 
 **order_by** | **str**|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1DescriptorsPaginatedItemsResponse**](EdfiAdminApiEdfiAdminV1DescriptorsPaginatedItemsResponse.md)

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

# **update_descriptor_async**
> EdfiAdminApiEdfiAdminV1DescriptorUpdatedResponse update_descriptor_async(tenant_id, instance_id, year, descriptor_id, edfi_admin_api_edfi_admin_v1_descriptor_type=edfi_admin_api_edfi_admin_v1_descriptor_type)

Updates a Descriptor.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_descriptor_type import EdfiAdminApiEdfiAdminV1DescriptorType
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_descriptor_updated_response import EdfiAdminApiEdfiAdminV1DescriptorUpdatedResponse
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
    api_instance = edgraph_platform_client.InstancesDescriptorsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    descriptor_id = 56 # int | 
    edfi_admin_api_edfi_admin_v1_descriptor_type = edgraph_platform_client.EdfiAdminApiEdfiAdminV1DescriptorType() # EdfiAdminApiEdfiAdminV1DescriptorType |  (optional)

    try:
        # Updates a Descriptor.
        api_response = api_instance.update_descriptor_async(tenant_id, instance_id, year, descriptor_id, edfi_admin_api_edfi_admin_v1_descriptor_type=edfi_admin_api_edfi_admin_v1_descriptor_type)
        print("The response of InstancesDescriptorsApi->update_descriptor_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesDescriptorsApi->update_descriptor_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **descriptor_id** | **int**|  | 
 **edfi_admin_api_edfi_admin_v1_descriptor_type** | [**EdfiAdminApiEdfiAdminV1DescriptorType**](EdfiAdminApiEdfiAdminV1DescriptorType.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1DescriptorUpdatedResponse**](EdfiAdminApiEdfiAdminV1DescriptorUpdatedResponse.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

