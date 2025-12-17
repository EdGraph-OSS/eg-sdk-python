# edgraph_platform_client.CollectionsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_collection**](CollectionsApi.md#create_collection) | **POST** /tenants/{tenantId}/validations/collections | Creates a Collection.
[**create_container**](CollectionsApi.md#create_container) | **POST** /tenants/{tenantId}/validations/collections/{collectionId}/containers | Creates a Container.
[**delete_collection**](CollectionsApi.md#delete_collection) | **DELETE** /tenants/{tenantId}/validations/collections/{collectionId} | Deletes a Collection.
[**delete_container**](CollectionsApi.md#delete_container) | **DELETE** /tenants/{tenantId}/validations/collections/{collectionId}/containers/{containerId} | Deletes a Container.
[**get_collection_by_id**](CollectionsApi.md#get_collection_by_id) | **GET** /tenants/{tenantId}/validations/collections/{collectionId} | Retrieves a Collection by ID.
[**get_collection_json**](CollectionsApi.md#get_collection_json) | **GET** /tenants/{tenantId}/validations/collections/{collectionId}/export | Retrieves the JSON representation of a Collection. Useful for exporting into other systems.
[**get_collections**](CollectionsApi.md#get_collections) | **GET** /tenants/{tenantId}/validations/collections | Retrieves a list of Collections.
[**get_collections_tree**](CollectionsApi.md#get_collections_tree) | **GET** /tenants/{tenantId}/validations/categories/tree | Retrieves a list of Collections.
[**get_container_by_id**](CollectionsApi.md#get_container_by_id) | **GET** /tenants/{tenantId}/validations/collections/{collectionId}/containers/{containerId} | Retrieves a Container by ID.
[**get_containers**](CollectionsApi.md#get_containers) | **GET** /tenants/{tenantId}/validations/collections/{collectionId}/containers | Retrieves a list of Containers.
[**update_collection**](CollectionsApi.md#update_collection) | **PUT** /tenants/{tenantId}/validations/collections/{collectionId} | Updates a Collection.
[**update_container**](CollectionsApi.md#update_container) | **PUT** /tenants/{tenantId}/validations/collections/{collectionId}/containers/{containerId} | Updates a Container.
[**upload_collection_json**](CollectionsApi.md#upload_collection_json) | **POST** /tenants/{tenantId}/validations/collections/import | Uploads a Collection JSON. Useful for importing from another system.


# **create_collection**
> ValidationsApiCoreV1CreatedResponse create_collection(tenant_id, validations_api_containers_v1_create_collection_request=validations_api_containers_v1_create_collection_request)

Creates a Collection.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_create_collection_request import ValidationsApiContainersV1CreateCollectionRequest
from edgraph_platform_client.models.validations_api_core_v1_created_response import ValidationsApiCoreV1CreatedResponse
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
    api_instance = edgraph_platform_client.CollectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    validations_api_containers_v1_create_collection_request = edgraph_platform_client.ValidationsApiContainersV1CreateCollectionRequest() # ValidationsApiContainersV1CreateCollectionRequest |  (optional)

    try:
        # Creates a Collection.
        api_response = api_instance.create_collection(tenant_id, validations_api_containers_v1_create_collection_request=validations_api_containers_v1_create_collection_request)
        print("The response of CollectionsApi->create_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->create_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **validations_api_containers_v1_create_collection_request** | [**ValidationsApiContainersV1CreateCollectionRequest**](ValidationsApiContainersV1CreateCollectionRequest.md)|  | [optional] 

### Return type

[**ValidationsApiCoreV1CreatedResponse**](ValidationsApiCoreV1CreatedResponse.md)

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

# **create_container**
> ValidationsApiCoreV1CreatedResponse create_container(tenant_id, collection_id, validations_api_containers_v1_create_container_request=validations_api_containers_v1_create_container_request)

Creates a Container.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_create_container_request import ValidationsApiContainersV1CreateContainerRequest
from edgraph_platform_client.models.validations_api_core_v1_created_response import ValidationsApiCoreV1CreatedResponse
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
    api_instance = edgraph_platform_client.CollectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    collection_id = 'collection_id_example' # str | 
    validations_api_containers_v1_create_container_request = edgraph_platform_client.ValidationsApiContainersV1CreateContainerRequest() # ValidationsApiContainersV1CreateContainerRequest |  (optional)

    try:
        # Creates a Container.
        api_response = api_instance.create_container(tenant_id, collection_id, validations_api_containers_v1_create_container_request=validations_api_containers_v1_create_container_request)
        print("The response of CollectionsApi->create_container:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->create_container: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **collection_id** | **str**|  | 
 **validations_api_containers_v1_create_container_request** | [**ValidationsApiContainersV1CreateContainerRequest**](ValidationsApiContainersV1CreateContainerRequest.md)|  | [optional] 

### Return type

[**ValidationsApiCoreV1CreatedResponse**](ValidationsApiCoreV1CreatedResponse.md)

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

# **delete_collection**
> delete_collection(tenant_id, collection_id)

Deletes a Collection.

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
    api_instance = edgraph_platform_client.CollectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    collection_id = 'collection_id_example' # str | 

    try:
        # Deletes a Collection.
        api_instance.delete_collection(tenant_id, collection_id)
    except Exception as e:
        print("Exception when calling CollectionsApi->delete_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **collection_id** | **str**|  | 

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

# **delete_container**
> delete_container(tenant_id, collection_id, container_id)

Deletes a Container.

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
    api_instance = edgraph_platform_client.CollectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    collection_id = 'collection_id_example' # str | 
    container_id = 'container_id_example' # str | 

    try:
        # Deletes a Container.
        api_instance.delete_container(tenant_id, collection_id, container_id)
    except Exception as e:
        print("Exception when calling CollectionsApi->delete_container: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **collection_id** | **str**|  | 
 **container_id** | **str**|  | 

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

# **get_collection_by_id**
> ValidationsApiContainersV1ContainerDto get_collection_by_id(tenant_id, collection_id)

Retrieves a Collection by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_container_dto import ValidationsApiContainersV1ContainerDto
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
    api_instance = edgraph_platform_client.CollectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    collection_id = 'collection_id_example' # str | 

    try:
        # Retrieves a Collection by ID.
        api_response = api_instance.get_collection_by_id(tenant_id, collection_id)
        print("The response of CollectionsApi->get_collection_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->get_collection_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **collection_id** | **str**|  | 

### Return type

[**ValidationsApiContainersV1ContainerDto**](ValidationsApiContainersV1ContainerDto.md)

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

# **get_collection_json**
> ValidationsApiContainersV1GetJsonResponse get_collection_json(tenant_id, collection_id)

Retrieves the JSON representation of a Collection. Useful for exporting into other systems.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_get_json_response import ValidationsApiContainersV1GetJsonResponse
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
    api_instance = edgraph_platform_client.CollectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    collection_id = 'collection_id_example' # str | 

    try:
        # Retrieves the JSON representation of a Collection. Useful for exporting into other systems.
        api_response = api_instance.get_collection_json(tenant_id, collection_id)
        print("The response of CollectionsApi->get_collection_json:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->get_collection_json: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **collection_id** | **str**|  | 

### Return type

[**ValidationsApiContainersV1GetJsonResponse**](ValidationsApiContainersV1GetJsonResponse.md)

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

# **get_collections**
> ValidationsApiContainersV1PaginatedContainers get_collections(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)

Retrieves a list of Collections.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_paginated_containers import ValidationsApiContainersV1PaginatedContainers
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
    api_instance = edgraph_platform_client.CollectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    filter = 'filter_example' # str |  (optional)
    order_by = 'order_by_example' # str |  (optional)

    try:
        # Retrieves a list of Collections.
        api_response = api_instance.get_collections(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)
        print("The response of CollectionsApi->get_collections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->get_collections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **filter** | **str**|  | [optional] 
 **order_by** | **str**|  | [optional] 

### Return type

[**ValidationsApiContainersV1PaginatedContainers**](ValidationsApiContainersV1PaginatedContainers.md)

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

# **get_collections_tree**
> ValidationsApiContainersV1PaginatedCategoryTreeResponse get_collections_tree(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, category_id=category_id, category_name=category_name, sub_category_id=sub_category_id, sub_category_name=sub_category_name)

Retrieves a list of Collections.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_paginated_category_tree_response import ValidationsApiContainersV1PaginatedCategoryTreeResponse
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
    api_instance = edgraph_platform_client.CollectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = 'order_by_example' # str |  (optional)
    category_id = 'category_id_example' # str |  (optional)
    category_name = 'category_name_example' # str |  (optional)
    sub_category_id = 'sub_category_id_example' # str |  (optional)
    sub_category_name = 'sub_category_name_example' # str |  (optional)

    try:
        # Retrieves a list of Collections.
        api_response = api_instance.get_collections_tree(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, category_id=category_id, category_name=category_name, sub_category_id=sub_category_id, sub_category_name=sub_category_name)
        print("The response of CollectionsApi->get_collections_tree:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->get_collections_tree: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **order_by** | **str**|  | [optional] 
 **category_id** | **str**|  | [optional] 
 **category_name** | **str**|  | [optional] 
 **sub_category_id** | **str**|  | [optional] 
 **sub_category_name** | **str**|  | [optional] 

### Return type

[**ValidationsApiContainersV1PaginatedCategoryTreeResponse**](ValidationsApiContainersV1PaginatedCategoryTreeResponse.md)

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

# **get_container_by_id**
> ValidationsApiContainersV1ContainerDto get_container_by_id(tenant_id, collection_id, container_id)

Retrieves a Container by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_container_dto import ValidationsApiContainersV1ContainerDto
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
    api_instance = edgraph_platform_client.CollectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    collection_id = 'collection_id_example' # str | 
    container_id = 'container_id_example' # str | 

    try:
        # Retrieves a Container by ID.
        api_response = api_instance.get_container_by_id(tenant_id, collection_id, container_id)
        print("The response of CollectionsApi->get_container_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->get_container_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **collection_id** | **str**|  | 
 **container_id** | **str**|  | 

### Return type

[**ValidationsApiContainersV1ContainerDto**](ValidationsApiContainersV1ContainerDto.md)

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

# **get_containers**
> ValidationsApiContainersV1PaginatedContainers get_containers(tenant_id, collection_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)

Retrieves a list of Containers.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_paginated_containers import ValidationsApiContainersV1PaginatedContainers
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
    api_instance = edgraph_platform_client.CollectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    collection_id = 'collection_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    filter = 'filter_example' # str |  (optional)
    order_by = 'order_by_example' # str |  (optional)

    try:
        # Retrieves a list of Containers.
        api_response = api_instance.get_containers(tenant_id, collection_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)
        print("The response of CollectionsApi->get_containers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->get_containers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **collection_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **filter** | **str**|  | [optional] 
 **order_by** | **str**|  | [optional] 

### Return type

[**ValidationsApiContainersV1PaginatedContainers**](ValidationsApiContainersV1PaginatedContainers.md)

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

# **update_collection**
> update_collection(tenant_id, collection_id, validations_api_containers_v1_update_collection_request=validations_api_containers_v1_update_collection_request)

Updates a Collection.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_update_collection_request import ValidationsApiContainersV1UpdateCollectionRequest
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
    api_instance = edgraph_platform_client.CollectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    collection_id = 'collection_id_example' # str | 
    validations_api_containers_v1_update_collection_request = edgraph_platform_client.ValidationsApiContainersV1UpdateCollectionRequest() # ValidationsApiContainersV1UpdateCollectionRequest |  (optional)

    try:
        # Updates a Collection.
        api_instance.update_collection(tenant_id, collection_id, validations_api_containers_v1_update_collection_request=validations_api_containers_v1_update_collection_request)
    except Exception as e:
        print("Exception when calling CollectionsApi->update_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **collection_id** | **str**|  | 
 **validations_api_containers_v1_update_collection_request** | [**ValidationsApiContainersV1UpdateCollectionRequest**](ValidationsApiContainersV1UpdateCollectionRequest.md)|  | [optional] 

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
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_container**
> update_container(tenant_id, collection_id, container_id, validations_api_containers_v1_update_container_request=validations_api_containers_v1_update_container_request)

Updates a Container.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_update_container_request import ValidationsApiContainersV1UpdateContainerRequest
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
    api_instance = edgraph_platform_client.CollectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    collection_id = 'collection_id_example' # str | 
    container_id = 'container_id_example' # str | 
    validations_api_containers_v1_update_container_request = edgraph_platform_client.ValidationsApiContainersV1UpdateContainerRequest() # ValidationsApiContainersV1UpdateContainerRequest |  (optional)

    try:
        # Updates a Container.
        api_instance.update_container(tenant_id, collection_id, container_id, validations_api_containers_v1_update_container_request=validations_api_containers_v1_update_container_request)
    except Exception as e:
        print("Exception when calling CollectionsApi->update_container: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **collection_id** | **str**|  | 
 **container_id** | **str**|  | 
 **validations_api_containers_v1_update_container_request** | [**ValidationsApiContainersV1UpdateContainerRequest**](ValidationsApiContainersV1UpdateContainerRequest.md)|  | [optional] 

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
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **upload_collection_json**
> ValidationsApiContainersV1CollectionUploadedResponse upload_collection_json(tenant_id, validations_api_containers_v1_upload_collection_request=validations_api_containers_v1_upload_collection_request)

Uploads a Collection JSON. Useful for importing from another system.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_containers_v1_collection_uploaded_response import ValidationsApiContainersV1CollectionUploadedResponse
from edgraph_platform_client.models.validations_api_containers_v1_upload_collection_request import ValidationsApiContainersV1UploadCollectionRequest
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
    api_instance = edgraph_platform_client.CollectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    validations_api_containers_v1_upload_collection_request = edgraph_platform_client.ValidationsApiContainersV1UploadCollectionRequest() # ValidationsApiContainersV1UploadCollectionRequest |  (optional)

    try:
        # Uploads a Collection JSON. Useful for importing from another system.
        api_response = api_instance.upload_collection_json(tenant_id, validations_api_containers_v1_upload_collection_request=validations_api_containers_v1_upload_collection_request)
        print("The response of CollectionsApi->upload_collection_json:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->upload_collection_json: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **validations_api_containers_v1_upload_collection_request** | [**ValidationsApiContainersV1UploadCollectionRequest**](ValidationsApiContainersV1UploadCollectionRequest.md)|  | [optional] 

### Return type

[**ValidationsApiContainersV1CollectionUploadedResponse**](ValidationsApiContainersV1CollectionUploadedResponse.md)

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

