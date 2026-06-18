# edgraph_platform_client.InstancesEducationOrganizationsLocalEducationAgenciesApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_local_education_agency_async**](InstancesEducationOrganizationsLocalEducationAgenciesApi.md#create_local_education_agency_async) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/localeducationagencies | Creates a LocalEducationAgency.
[**delete_local_education_agency_async**](InstancesEducationOrganizationsLocalEducationAgenciesApi.md#delete_local_education_agency_async) | **DELETE** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/localeducationagencies/{localEducationAgencyId} | Deletes a LocalEducationAgency.
[**get_local_education_agency_by_id_async**](InstancesEducationOrganizationsLocalEducationAgenciesApi.md#get_local_education_agency_by_id_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/localeducationagencies/{localEducationAgencyId} | Retrieves a LocalEducationAgency by ID.
[**getl_local_education_agencies_async**](InstancesEducationOrganizationsLocalEducationAgenciesApi.md#getl_local_education_agencies_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/localeducationagencies | Retrieves a list of LocalEducationAgencies.
[**sync_local_education_agency_async**](InstancesEducationOrganizationsLocalEducationAgenciesApi.md#sync_local_education_agency_async) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/localeducationagencies/{localEducationAgencyId}/sync | Copies a LocalEducationAgency from one instance to another/other instance(s).
[**update_local_education_agency_async**](InstancesEducationOrganizationsLocalEducationAgenciesApi.md#update_local_education_agency_async) | **PUT** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/localeducationagencies/{localEducationAgencyId} | Updates a LocalEducationAgency.


# **create_local_education_agency_async**
> EdfiAdminApiEdfiAdminV1LocalEducationAgencyCreatedResponse create_local_education_agency_async(tenant_id, instance_id, year, edfi_admin_api_edfi_admin_v1_create_local_education_agency_request=edfi_admin_api_edfi_admin_v1_create_local_education_agency_request)

Creates a LocalEducationAgency.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_local_education_agency_request import EdfiAdminApiEdfiAdminV1CreateLocalEducationAgencyRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_local_education_agency_created_response import EdfiAdminApiEdfiAdminV1LocalEducationAgencyCreatedResponse
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
    api_instance = edgraph_platform_client.InstancesEducationOrganizationsLocalEducationAgenciesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    edfi_admin_api_edfi_admin_v1_create_local_education_agency_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1CreateLocalEducationAgencyRequest() # EdfiAdminApiEdfiAdminV1CreateLocalEducationAgencyRequest |  (optional)

    try:
        # Creates a LocalEducationAgency.
        api_response = await api_instance.create_local_education_agency_async(tenant_id, instance_id, year, edfi_admin_api_edfi_admin_v1_create_local_education_agency_request=edfi_admin_api_edfi_admin_v1_create_local_education_agency_request)
        print("The response of InstancesEducationOrganizationsLocalEducationAgenciesApi->create_local_education_agency_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesEducationOrganizationsLocalEducationAgenciesApi->create_local_education_agency_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **edfi_admin_api_edfi_admin_v1_create_local_education_agency_request** | [**EdfiAdminApiEdfiAdminV1CreateLocalEducationAgencyRequest**](EdfiAdminApiEdfiAdminV1CreateLocalEducationAgencyRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1LocalEducationAgencyCreatedResponse**](EdfiAdminApiEdfiAdminV1LocalEducationAgencyCreatedResponse.md)

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

# **delete_local_education_agency_async**
> delete_local_education_agency_async(tenant_id, instance_id, year, local_education_agency_id)

Deletes a LocalEducationAgency.

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
    api_instance = edgraph_platform_client.InstancesEducationOrganizationsLocalEducationAgenciesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    local_education_agency_id = 'local_education_agency_id_example' # str | 

    try:
        # Deletes a LocalEducationAgency.
        await api_instance.delete_local_education_agency_async(tenant_id, instance_id, year, local_education_agency_id)
    except Exception as e:
        print("Exception when calling InstancesEducationOrganizationsLocalEducationAgenciesApi->delete_local_education_agency_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **local_education_agency_id** | **str**|  | 

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

# **get_local_education_agency_by_id_async**
> EdfiAdminApiEdfiAdminV1GetLocalEducationAgencyProfileResponse get_local_education_agency_by_id_async(tenant_id, instance_id, year, local_education_agency_id)

Retrieves a LocalEducationAgency by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_get_local_education_agency_profile_response import EdfiAdminApiEdfiAdminV1GetLocalEducationAgencyProfileResponse
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
    api_instance = edgraph_platform_client.InstancesEducationOrganizationsLocalEducationAgenciesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    local_education_agency_id = 'local_education_agency_id_example' # str | 

    try:
        # Retrieves a LocalEducationAgency by ID.
        api_response = await api_instance.get_local_education_agency_by_id_async(tenant_id, instance_id, year, local_education_agency_id)
        print("The response of InstancesEducationOrganizationsLocalEducationAgenciesApi->get_local_education_agency_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesEducationOrganizationsLocalEducationAgenciesApi->get_local_education_agency_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **local_education_agency_id** | **str**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1GetLocalEducationAgencyProfileResponse**](EdfiAdminApiEdfiAdminV1GetLocalEducationAgencyProfileResponse.md)

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

# **getl_local_education_agencies_async**
> EdfiAdminApiEdfiAdminV1LocalEducationAgencyTableViewResponsePaginatedItemsViewModel getl_local_education_agencies_async(tenant_id, instance_id, year, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of LocalEducationAgencies.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_local_education_agency_table_view_response_paginated_items_view_model import EdfiAdminApiEdfiAdminV1LocalEducationAgencyTableViewResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.InstancesEducationOrganizationsLocalEducationAgenciesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of LocalEducationAgencies.
        api_response = await api_instance.getl_local_education_agencies_async(tenant_id, instance_id, year, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of InstancesEducationOrganizationsLocalEducationAgenciesApi->getl_local_education_agencies_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesEducationOrganizationsLocalEducationAgenciesApi->getl_local_education_agencies_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdfiAdminApiEdfiAdminV1LocalEducationAgencyTableViewResponsePaginatedItemsViewModel**](EdfiAdminApiEdfiAdminV1LocalEducationAgencyTableViewResponsePaginatedItemsViewModel.md)

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

# **sync_local_education_agency_async**
> EdfiAdminApiEdfiAdminV1SyncResponse sync_local_education_agency_async(tenant_id, instance_id, year, local_education_agency_id, edfi_admin_api_edfi_admin_v1_sync_local_education_agency_request=edfi_admin_api_edfi_admin_v1_sync_local_education_agency_request)

Copies a LocalEducationAgency from one instance to another/other instance(s).

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_sync_local_education_agency_request import EdfiAdminApiEdfiAdminV1SyncLocalEducationAgencyRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_sync_response import EdfiAdminApiEdfiAdminV1SyncResponse
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
    api_instance = edgraph_platform_client.InstancesEducationOrganizationsLocalEducationAgenciesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    local_education_agency_id = 56 # int | 
    edfi_admin_api_edfi_admin_v1_sync_local_education_agency_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1SyncLocalEducationAgencyRequest() # EdfiAdminApiEdfiAdminV1SyncLocalEducationAgencyRequest |  (optional)

    try:
        # Copies a LocalEducationAgency from one instance to another/other instance(s).
        api_response = await api_instance.sync_local_education_agency_async(tenant_id, instance_id, year, local_education_agency_id, edfi_admin_api_edfi_admin_v1_sync_local_education_agency_request=edfi_admin_api_edfi_admin_v1_sync_local_education_agency_request)
        print("The response of InstancesEducationOrganizationsLocalEducationAgenciesApi->sync_local_education_agency_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesEducationOrganizationsLocalEducationAgenciesApi->sync_local_education_agency_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **local_education_agency_id** | **int**|  | 
 **edfi_admin_api_edfi_admin_v1_sync_local_education_agency_request** | [**EdfiAdminApiEdfiAdminV1SyncLocalEducationAgencyRequest**](EdfiAdminApiEdfiAdminV1SyncLocalEducationAgencyRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1SyncResponse**](EdfiAdminApiEdfiAdminV1SyncResponse.md)

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

# **update_local_education_agency_async**
> update_local_education_agency_async(tenant_id, instance_id, year, local_education_agency_id, edfi_admin_api_edfi_admin_v1_update_local_education_agency_request=edfi_admin_api_edfi_admin_v1_update_local_education_agency_request)

Updates a LocalEducationAgency.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_local_education_agency_request import EdfiAdminApiEdfiAdminV1UpdateLocalEducationAgencyRequest
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
    api_instance = edgraph_platform_client.InstancesEducationOrganizationsLocalEducationAgenciesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    local_education_agency_id = 'local_education_agency_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_update_local_education_agency_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1UpdateLocalEducationAgencyRequest() # EdfiAdminApiEdfiAdminV1UpdateLocalEducationAgencyRequest |  (optional)

    try:
        # Updates a LocalEducationAgency.
        await api_instance.update_local_education_agency_async(tenant_id, instance_id, year, local_education_agency_id, edfi_admin_api_edfi_admin_v1_update_local_education_agency_request=edfi_admin_api_edfi_admin_v1_update_local_education_agency_request)
    except Exception as e:
        print("Exception when calling InstancesEducationOrganizationsLocalEducationAgenciesApi->update_local_education_agency_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **local_education_agency_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_update_local_education_agency_request** | [**EdfiAdminApiEdfiAdminV1UpdateLocalEducationAgencyRequest**](EdfiAdminApiEdfiAdminV1UpdateLocalEducationAgencyRequest.md)|  | [optional] 

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

