# edgraph_platform_client.InstancesDescriptorMappingsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_descriptor_mapping**](InstancesDescriptorMappingsApi.md#create_descriptor_mapping) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/descriptorMappings | Creates a Descriptor Mapping.
[**delete_descriptor_mapping**](InstancesDescriptorMappingsApi.md#delete_descriptor_mapping) | **DELETE** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/descriptorMappings/{descriptorMappingId} | Deletes a Descriptor Mapping.
[**get_descriptor_mapping_by_id**](InstancesDescriptorMappingsApi.md#get_descriptor_mapping_by_id) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/descriptorMappings/{descriptorMappingId} | Retrieves a Descriptor Mapping by ID.
[**get_descriptor_mappings**](InstancesDescriptorMappingsApi.md#get_descriptor_mappings) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/descriptorMappings | Retrieves a list of Descriptors Mappings.
[**update_descriptor_mapping**](InstancesDescriptorMappingsApi.md#update_descriptor_mapping) | **PUT** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/descriptorMappings/{descriptorMappingId} | Updates a Descriptor Mapping.


# **create_descriptor_mapping**
> EdfiAdminApiEdfiAdminV1DescriptorMappingCreatedResponse create_descriptor_mapping(tenant_id, instance_id, year, edfi_admin_api_edfi_admin_v1_create_descriptor_mapping_request=edfi_admin_api_edfi_admin_v1_create_descriptor_mapping_request)

Creates a Descriptor Mapping.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_descriptor_mapping_request import EdfiAdminApiEdfiAdminV1CreateDescriptorMappingRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_descriptor_mapping_created_response import EdfiAdminApiEdfiAdminV1DescriptorMappingCreatedResponse
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
    api_instance = edgraph_platform_client.InstancesDescriptorMappingsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    edfi_admin_api_edfi_admin_v1_create_descriptor_mapping_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1CreateDescriptorMappingRequest() # EdfiAdminApiEdfiAdminV1CreateDescriptorMappingRequest |  (optional)

    try:
        # Creates a Descriptor Mapping.
        api_response = api_instance.create_descriptor_mapping(tenant_id, instance_id, year, edfi_admin_api_edfi_admin_v1_create_descriptor_mapping_request=edfi_admin_api_edfi_admin_v1_create_descriptor_mapping_request)
        print("The response of InstancesDescriptorMappingsApi->create_descriptor_mapping:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesDescriptorMappingsApi->create_descriptor_mapping: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **edfi_admin_api_edfi_admin_v1_create_descriptor_mapping_request** | [**EdfiAdminApiEdfiAdminV1CreateDescriptorMappingRequest**](EdfiAdminApiEdfiAdminV1CreateDescriptorMappingRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1DescriptorMappingCreatedResponse**](EdfiAdminApiEdfiAdminV1DescriptorMappingCreatedResponse.md)

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

# **delete_descriptor_mapping**
> delete_descriptor_mapping(tenant_id, instance_id, year, descriptor_mapping_id)

Deletes a Descriptor Mapping.

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
    api_instance = edgraph_platform_client.InstancesDescriptorMappingsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    descriptor_mapping_id = 'descriptor_mapping_id_example' # str | 

    try:
        # Deletes a Descriptor Mapping.
        api_instance.delete_descriptor_mapping(tenant_id, instance_id, year, descriptor_mapping_id)
    except Exception as e:
        print("Exception when calling InstancesDescriptorMappingsApi->delete_descriptor_mapping: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **descriptor_mapping_id** | **str**|  | 

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

# **get_descriptor_mapping_by_id**
> EdfiAdminApiEdfiAdminV1DescriptorMapping get_descriptor_mapping_by_id(tenant_id, instance_id, year, descriptor_mapping_id)

Retrieves a Descriptor Mapping by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_descriptor_mapping import EdfiAdminApiEdfiAdminV1DescriptorMapping
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
    api_instance = edgraph_platform_client.InstancesDescriptorMappingsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    descriptor_mapping_id = 'descriptor_mapping_id_example' # str | 

    try:
        # Retrieves a Descriptor Mapping by ID.
        api_response = api_instance.get_descriptor_mapping_by_id(tenant_id, instance_id, year, descriptor_mapping_id)
        print("The response of InstancesDescriptorMappingsApi->get_descriptor_mapping_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesDescriptorMappingsApi->get_descriptor_mapping_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **descriptor_mapping_id** | **str**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1DescriptorMapping**](EdfiAdminApiEdfiAdminV1DescriptorMapping.md)

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

# **get_descriptor_mappings**
> EdfiAdminApiEdfiAdminV1DescriptorMappingsPaginatedItemsResponse get_descriptor_mappings(tenant_id, instance_id, year, page_size=page_size, page_index=page_index, namespace=namespace)

Retrieves a list of Descriptors Mappings.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_descriptor_mappings_paginated_items_response import EdfiAdminApiEdfiAdminV1DescriptorMappingsPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.InstancesDescriptorMappingsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    namespace = 'namespace_example' # str |  (optional)

    try:
        # Retrieves a list of Descriptors Mappings.
        api_response = api_instance.get_descriptor_mappings(tenant_id, instance_id, year, page_size=page_size, page_index=page_index, namespace=namespace)
        print("The response of InstancesDescriptorMappingsApi->get_descriptor_mappings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesDescriptorMappingsApi->get_descriptor_mappings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **namespace** | **str**|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1DescriptorMappingsPaginatedItemsResponse**](EdfiAdminApiEdfiAdminV1DescriptorMappingsPaginatedItemsResponse.md)

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

# **update_descriptor_mapping**
> EdfiAdminApiEdfiAdminV1DescriptorMappingUpdatedResponse update_descriptor_mapping(tenant_id, instance_id, year, descriptor_mapping_id, edfi_admin_api_edfi_admin_v1_update_descriptor_mapping_request=edfi_admin_api_edfi_admin_v1_update_descriptor_mapping_request)

Updates a Descriptor Mapping.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_descriptor_mapping_updated_response import EdfiAdminApiEdfiAdminV1DescriptorMappingUpdatedResponse
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_descriptor_mapping_request import EdfiAdminApiEdfiAdminV1UpdateDescriptorMappingRequest
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
    api_instance = edgraph_platform_client.InstancesDescriptorMappingsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    descriptor_mapping_id = 'descriptor_mapping_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_update_descriptor_mapping_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1UpdateDescriptorMappingRequest() # EdfiAdminApiEdfiAdminV1UpdateDescriptorMappingRequest |  (optional)

    try:
        # Updates a Descriptor Mapping.
        api_response = api_instance.update_descriptor_mapping(tenant_id, instance_id, year, descriptor_mapping_id, edfi_admin_api_edfi_admin_v1_update_descriptor_mapping_request=edfi_admin_api_edfi_admin_v1_update_descriptor_mapping_request)
        print("The response of InstancesDescriptorMappingsApi->update_descriptor_mapping:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesDescriptorMappingsApi->update_descriptor_mapping: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **descriptor_mapping_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_update_descriptor_mapping_request** | [**EdfiAdminApiEdfiAdminV1UpdateDescriptorMappingRequest**](EdfiAdminApiEdfiAdminV1UpdateDescriptorMappingRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1DescriptorMappingUpdatedResponse**](EdfiAdminApiEdfiAdminV1DescriptorMappingUpdatedResponse.md)

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

