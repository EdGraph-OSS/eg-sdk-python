# edgraph_platform_client.InstancesApplicationsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_application_async**](InstancesApplicationsApi.md#create_application_async) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/applications | Creates an Application.
[**create_application_user_access_async**](InstancesApplicationsApi.md#create_application_user_access_async) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/applications/{applicationId}/apiclients/{apiClientId}/access | Creates a new application access.
[**delete_application_async**](InstancesApplicationsApi.md#delete_application_async) | **DELETE** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/applications/{applicationId} | Deletes an Application.
[**delete_application_user_access_async**](InstancesApplicationsApi.md#delete_application_user_access_async) | **DELETE** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/applications/{applicationId}/apiclients/{apiClientId}/access/{accessId} | Deletes an application user access.
[**get_application_access_async**](InstancesApplicationsApi.md#get_application_access_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/applications/{applicationId}/apiclients/{apiClientId}/access | Retrieves a list of application accesses.
[**get_application_access_by_id_async**](InstancesApplicationsApi.md#get_application_access_by_id_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/applications/{applicationId}/apiclients/{apiClientId}/access/{accessId} | Retrieves an application access by ID.
[**get_application_api_client_by_id_async**](InstancesApplicationsApi.md#get_application_api_client_by_id_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/applications/{applicationId}/apiclients/{apiClientId} | Retrieves an API Client of an Application by ID.
[**get_application_api_clients_async**](InstancesApplicationsApi.md#get_application_api_clients_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/applications/{applicationId}/apiclients | Retrieves the API Clients of an Application.
[**get_application_by_id_async**](InstancesApplicationsApi.md#get_application_by_id_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/applications/{applicationId} | Retrieves an Application by ID.
[**get_applications_async**](InstancesApplicationsApi.md#get_applications_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/applications | Retrieves a list of Applications.
[**regenerate_api_client_secret_async**](InstancesApplicationsApi.md#regenerate_api_client_secret_async) | **PUT** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/applications/{applicationId}/apiclients/{apiClientId}/regenerate | Regenerates the secret of an API Client.
[**sync_application_async**](InstancesApplicationsApi.md#sync_application_async) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/applications/{applicationId}/sync | Copies an Application from one instance to another/other instance(s)
[**update_application_async**](InstancesApplicationsApi.md#update_application_async) | **PUT** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/applications/{applicationId} | Updates an Application.
[**update_application_user_access_async**](InstancesApplicationsApi.md#update_application_user_access_async) | **PUT** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/applications/{applicationId}/apiclients/{apiClientId}/access/{accessId} | Updates a new application access.


# **create_application_async**
> EdfiAdminApiEdfiAdminV1EdFiApplicationCreatedResponse create_application_async(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_create_ed_fi_application_request=edfi_admin_api_edfi_admin_v1_create_ed_fi_application_request)

Creates an Application.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_ed_fi_application_request import EdfiAdminApiEdfiAdminV1CreateEdFiApplicationRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ed_fi_application_created_response import EdfiAdminApiEdfiAdminV1EdFiApplicationCreatedResponse
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
    api_instance = edgraph_platform_client.InstancesApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_create_ed_fi_application_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1CreateEdFiApplicationRequest() # EdfiAdminApiEdfiAdminV1CreateEdFiApplicationRequest |  (optional)

    try:
        # Creates an Application.
        api_response = api_instance.create_application_async(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_create_ed_fi_application_request=edfi_admin_api_edfi_admin_v1_create_ed_fi_application_request)
        print("The response of InstancesApplicationsApi->create_application_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApplicationsApi->create_application_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_create_ed_fi_application_request** | [**EdfiAdminApiEdfiAdminV1CreateEdFiApplicationRequest**](EdfiAdminApiEdfiAdminV1CreateEdFiApplicationRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1EdFiApplicationCreatedResponse**](EdfiAdminApiEdfiAdminV1EdFiApplicationCreatedResponse.md)

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

# **create_application_user_access_async**
> create_application_user_access_async(tenant_id, instance_id, application_id, api_client_id, ed_fi_admin_api_application_access_v1_create_application_access_request=ed_fi_admin_api_application_access_v1_create_application_access_request)

Creates a new application access.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_fi_admin_api_application_access_v1_create_application_access_request import EdFiAdminApiApplicationAccessV1CreateApplicationAccessRequest
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
    api_instance = edgraph_platform_client.InstancesApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 'application_id_example' # str | 
    api_client_id = 'api_client_id_example' # str | 
    ed_fi_admin_api_application_access_v1_create_application_access_request = edgraph_platform_client.EdFiAdminApiApplicationAccessV1CreateApplicationAccessRequest() # EdFiAdminApiApplicationAccessV1CreateApplicationAccessRequest |  (optional)

    try:
        # Creates a new application access.
        api_instance.create_application_user_access_async(tenant_id, instance_id, application_id, api_client_id, ed_fi_admin_api_application_access_v1_create_application_access_request=ed_fi_admin_api_application_access_v1_create_application_access_request)
    except Exception as e:
        print("Exception when calling InstancesApplicationsApi->create_application_user_access_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **str**|  | 
 **api_client_id** | **str**|  | 
 **ed_fi_admin_api_application_access_v1_create_application_access_request** | [**EdFiAdminApiApplicationAccessV1CreateApplicationAccessRequest**](EdFiAdminApiApplicationAccessV1CreateApplicationAccessRequest.md)|  | [optional] 

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
**200** | Success |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**201** | The resource was created. The location of the resource is available in the Location header of the response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_application_async**
> delete_application_async(tenant_id, instance_id, application_id)

Deletes an Application.

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
    api_instance = edgraph_platform_client.InstancesApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 56 # int | 

    try:
        # Deletes an Application.
        api_instance.delete_application_async(tenant_id, instance_id, application_id)
    except Exception as e:
        print("Exception when calling InstancesApplicationsApi->delete_application_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **int**|  | 

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

# **delete_application_user_access_async**
> delete_application_user_access_async(tenant_id, instance_id, application_id, api_client_id, access_id)

Deletes an application user access.

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
    api_instance = edgraph_platform_client.InstancesApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 'application_id_example' # str | 
    api_client_id = 'api_client_id_example' # str | 
    access_id = 'access_id_example' # str | 

    try:
        # Deletes an application user access.
        api_instance.delete_application_user_access_async(tenant_id, instance_id, application_id, api_client_id, access_id)
    except Exception as e:
        print("Exception when calling InstancesApplicationsApi->delete_application_user_access_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **str**|  | 
 **api_client_id** | **str**|  | 
 **access_id** | **str**|  | 

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

# **get_application_access_async**
> EdFiAdminApiApplicationAccessV1ApplicationAccessResponsePaginatedItemsViewModel get_application_access_async(tenant_id, instance_id, application_id, api_client_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of application accesses.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_fi_admin_api_application_access_v1_application_access_response_paginated_items_view_model import EdFiAdminApiApplicationAccessV1ApplicationAccessResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.InstancesApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 'application_id_example' # str | 
    api_client_id = 'api_client_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of application accesses.
        api_response = api_instance.get_application_access_async(tenant_id, instance_id, application_id, api_client_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of InstancesApplicationsApi->get_application_access_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApplicationsApi->get_application_access_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **str**|  | 
 **api_client_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdFiAdminApiApplicationAccessV1ApplicationAccessResponsePaginatedItemsViewModel**](EdFiAdminApiApplicationAccessV1ApplicationAccessResponsePaginatedItemsViewModel.md)

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

# **get_application_access_by_id_async**
> EdFiAdminApiApplicationAccessV1ApplicationAccessResponse get_application_access_by_id_async(tenant_id, instance_id, application_id, api_client_id, access_id)

Retrieves an application access by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_fi_admin_api_application_access_v1_application_access_response import EdFiAdminApiApplicationAccessV1ApplicationAccessResponse
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
    api_instance = edgraph_platform_client.InstancesApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 56 # int | 
    api_client_id = 56 # int | 
    access_id = 'access_id_example' # str | 

    try:
        # Retrieves an application access by ID.
        api_response = api_instance.get_application_access_by_id_async(tenant_id, instance_id, application_id, api_client_id, access_id)
        print("The response of InstancesApplicationsApi->get_application_access_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApplicationsApi->get_application_access_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **int**|  | 
 **api_client_id** | **int**|  | 
 **access_id** | **str**|  | 

### Return type

[**EdFiAdminApiApplicationAccessV1ApplicationAccessResponse**](EdFiAdminApiApplicationAccessV1ApplicationAccessResponse.md)

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

# **get_application_api_client_by_id_async**
> EdfiAdminApiEdfiAdminV1EdFiApplicationApiClientProfileResponse get_application_api_client_by_id_async(tenant_id, instance_id, application_id, api_client_id)

Retrieves an API Client of an Application by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ed_fi_application_api_client_profile_response import EdfiAdminApiEdfiAdminV1EdFiApplicationApiClientProfileResponse
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
    api_instance = edgraph_platform_client.InstancesApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 'application_id_example' # str | 
    api_client_id = 56 # int | 

    try:
        # Retrieves an API Client of an Application by ID.
        api_response = api_instance.get_application_api_client_by_id_async(tenant_id, instance_id, application_id, api_client_id)
        print("The response of InstancesApplicationsApi->get_application_api_client_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApplicationsApi->get_application_api_client_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **str**|  | 
 **api_client_id** | **int**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1EdFiApplicationApiClientProfileResponse**](EdfiAdminApiEdfiAdminV1EdFiApplicationApiClientProfileResponse.md)

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

# **get_application_api_clients_async**
> EdfiAdminApiEdfiAdminV1EdFiApplicationApiClientProfileResponsePaginatedItemsViewModel get_application_api_clients_async(tenant_id, instance_id, application_id)

Retrieves the API Clients of an Application.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ed_fi_application_api_client_profile_response_paginated_items_view_model import EdfiAdminApiEdfiAdminV1EdFiApplicationApiClientProfileResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.InstancesApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 'application_id_example' # str | 

    try:
        # Retrieves the API Clients of an Application.
        api_response = api_instance.get_application_api_clients_async(tenant_id, instance_id, application_id)
        print("The response of InstancesApplicationsApi->get_application_api_clients_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApplicationsApi->get_application_api_clients_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **str**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1EdFiApplicationApiClientProfileResponsePaginatedItemsViewModel**](EdfiAdminApiEdfiAdminV1EdFiApplicationApiClientProfileResponsePaginatedItemsViewModel.md)

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

# **get_application_by_id_async**
> EdfiAdminApiEdfiAdminV1EdFiApplicationProfileResponse get_application_by_id_async(tenant_id, instance_id, application_id, year=year, load_education_organizations=load_education_organizations)

Retrieves an Application by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ed_fi_application_profile_response import EdfiAdminApiEdfiAdminV1EdFiApplicationProfileResponse
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
    api_instance = edgraph_platform_client.InstancesApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 56 # int | 
    year = 56 # int |  (optional)
    load_education_organizations = True # bool |  (optional)

    try:
        # Retrieves an Application by ID.
        api_response = api_instance.get_application_by_id_async(tenant_id, instance_id, application_id, year=year, load_education_organizations=load_education_organizations)
        print("The response of InstancesApplicationsApi->get_application_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApplicationsApi->get_application_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **int**|  | 
 **year** | **int**|  | [optional] 
 **load_education_organizations** | **bool**|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1EdFiApplicationProfileResponse**](EdfiAdminApiEdfiAdminV1EdFiApplicationProfileResponse.md)

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

# **get_applications_async**
> EdfiAdminApiEdfiAdminV1EdFiApplicationListResponsePaginatedItemsViewModel get_applications_async(tenant_id, instance_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of Applications.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ed_fi_application_list_response_paginated_items_view_model import EdfiAdminApiEdfiAdminV1EdFiApplicationListResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.InstancesApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of Applications.
        api_response = api_instance.get_applications_async(tenant_id, instance_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of InstancesApplicationsApi->get_applications_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApplicationsApi->get_applications_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdfiAdminApiEdfiAdminV1EdFiApplicationListResponsePaginatedItemsViewModel**](EdfiAdminApiEdfiAdminV1EdFiApplicationListResponsePaginatedItemsViewModel.md)

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

# **regenerate_api_client_secret_async**
> EdfiAdminApiEdfiAdminV1RegenerateApiClientSecretResponse regenerate_api_client_secret_async(tenant_id, instance_id, application_id, api_client_id)

Regenerates the secret of an API Client.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_regenerate_api_client_secret_response import EdfiAdminApiEdfiAdminV1RegenerateApiClientSecretResponse
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
    api_instance = edgraph_platform_client.InstancesApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 56 # int | 
    api_client_id = 56 # int | 

    try:
        # Regenerates the secret of an API Client.
        api_response = api_instance.regenerate_api_client_secret_async(tenant_id, instance_id, application_id, api_client_id)
        print("The response of InstancesApplicationsApi->regenerate_api_client_secret_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesApplicationsApi->regenerate_api_client_secret_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **int**|  | 
 **api_client_id** | **int**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1RegenerateApiClientSecretResponse**](EdfiAdminApiEdfiAdminV1RegenerateApiClientSecretResponse.md)

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

# **sync_application_async**
> sync_application_async(tenant_id, instance_id, application_id, edfi_admin_api_edfi_admin_v1_sync_application_request=edfi_admin_api_edfi_admin_v1_sync_application_request)

Copies an Application from one instance to another/other instance(s)

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_sync_application_request import EdfiAdminApiEdfiAdminV1SyncApplicationRequest
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
    api_instance = edgraph_platform_client.InstancesApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 56 # int | 
    edfi_admin_api_edfi_admin_v1_sync_application_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1SyncApplicationRequest() # EdfiAdminApiEdfiAdminV1SyncApplicationRequest |  (optional)

    try:
        # Copies an Application from one instance to another/other instance(s)
        api_instance.sync_application_async(tenant_id, instance_id, application_id, edfi_admin_api_edfi_admin_v1_sync_application_request=edfi_admin_api_edfi_admin_v1_sync_application_request)
    except Exception as e:
        print("Exception when calling InstancesApplicationsApi->sync_application_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **int**|  | 
 **edfi_admin_api_edfi_admin_v1_sync_application_request** | [**EdfiAdminApiEdfiAdminV1SyncApplicationRequest**](EdfiAdminApiEdfiAdminV1SyncApplicationRequest.md)|  | [optional] 

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

# **update_application_async**
> update_application_async(tenant_id, instance_id, application_id, edfi_admin_api_edfi_admin_v1_update_ed_fi_application_request=edfi_admin_api_edfi_admin_v1_update_ed_fi_application_request)

Updates an Application.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_ed_fi_application_request import EdfiAdminApiEdfiAdminV1UpdateEdFiApplicationRequest
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
    api_instance = edgraph_platform_client.InstancesApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 'application_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_update_ed_fi_application_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1UpdateEdFiApplicationRequest() # EdfiAdminApiEdfiAdminV1UpdateEdFiApplicationRequest |  (optional)

    try:
        # Updates an Application.
        api_instance.update_application_async(tenant_id, instance_id, application_id, edfi_admin_api_edfi_admin_v1_update_ed_fi_application_request=edfi_admin_api_edfi_admin_v1_update_ed_fi_application_request)
    except Exception as e:
        print("Exception when calling InstancesApplicationsApi->update_application_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_update_ed_fi_application_request** | [**EdfiAdminApiEdfiAdminV1UpdateEdFiApplicationRequest**](EdfiAdminApiEdfiAdminV1UpdateEdFiApplicationRequest.md)|  | [optional] 

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

# **update_application_user_access_async**
> update_application_user_access_async(tenant_id, instance_id, application_id, api_client_id, access_id, ed_fi_admin_api_application_access_v1_update_application_access_request=ed_fi_admin_api_application_access_v1_update_application_access_request)

Updates a new application access.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_fi_admin_api_application_access_v1_update_application_access_request import EdFiAdminApiApplicationAccessV1UpdateApplicationAccessRequest
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
    api_instance = edgraph_platform_client.InstancesApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 'application_id_example' # str | 
    api_client_id = 'api_client_id_example' # str | 
    access_id = 'access_id_example' # str | 
    ed_fi_admin_api_application_access_v1_update_application_access_request = edgraph_platform_client.EdFiAdminApiApplicationAccessV1UpdateApplicationAccessRequest() # EdFiAdminApiApplicationAccessV1UpdateApplicationAccessRequest |  (optional)

    try:
        # Updates a new application access.
        api_instance.update_application_user_access_async(tenant_id, instance_id, application_id, api_client_id, access_id, ed_fi_admin_api_application_access_v1_update_application_access_request=ed_fi_admin_api_application_access_v1_update_application_access_request)
    except Exception as e:
        print("Exception when calling InstancesApplicationsApi->update_application_user_access_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **str**|  | 
 **api_client_id** | **str**|  | 
 **access_id** | **str**|  | 
 **ed_fi_admin_api_application_access_v1_update_application_access_request** | [**EdFiAdminApiApplicationAccessV1UpdateApplicationAccessRequest**](EdFiAdminApiApplicationAccessV1UpdateApplicationAccessRequest.md)|  | [optional] 

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
**200** | Success |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**201** | The resource was created. The location of the resource is available in the Location header of the response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

