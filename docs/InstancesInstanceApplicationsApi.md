# edgraph_platform_client.InstancesInstanceApplicationsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_instance_application**](InstancesInstanceApplicationsApi.md#create_instance_application) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/instanceapplications | Creates an Instance Application
[**delete_instance_application**](InstancesInstanceApplicationsApi.md#delete_instance_application) | **DELETE** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/instanceapplications/{applicationId} | Deletes an Instance Application
[**get_instance_application_by_id**](InstancesInstanceApplicationsApi.md#get_instance_application_by_id) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/instanceapplications/{applicationId} | Retrieves an Instance Application by ID.
[**get_instance_applications**](InstancesInstanceApplicationsApi.md#get_instance_applications) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/instanceapplications | Retrieves a paginated list of Instance applications
[**update_instance_application**](InstancesInstanceApplicationsApi.md#update_instance_application) | **PUT** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/instanceapplications/{applicationId} | Updates an Instance Application


# **create_instance_application**
> EdfiAdminApiEdfiAdminV1InstanceApplicationCreatedResponse create_instance_application(tenant_id, instance_id, ed_graph_http_aggregators_tenant_api_services_instance_applications_use_cases_create_tenant_instance_application_request=ed_graph_http_aggregators_tenant_api_services_instance_applications_use_cases_create_tenant_instance_application_request)

Creates an Instance Application

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_instance_applications_use_cases_create_tenant_instance_application_request import EdGraphHttpAggregatorsTenantApiServicesInstanceApplicationsUseCasesCreateTenantInstanceApplicationRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_application_created_response import EdfiAdminApiEdfiAdminV1InstanceApplicationCreatedResponse
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
    api_instance = edgraph_platform_client.InstancesInstanceApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_services_instance_applications_use_cases_create_tenant_instance_application_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesInstanceApplicationsUseCasesCreateTenantInstanceApplicationRequest() # EdGraphHttpAggregatorsTenantApiServicesInstanceApplicationsUseCasesCreateTenantInstanceApplicationRequest |  (optional)

    try:
        # Creates an Instance Application
        api_response = api_instance.create_instance_application(tenant_id, instance_id, ed_graph_http_aggregators_tenant_api_services_instance_applications_use_cases_create_tenant_instance_application_request=ed_graph_http_aggregators_tenant_api_services_instance_applications_use_cases_create_tenant_instance_application_request)
        print("The response of InstancesInstanceApplicationsApi->create_instance_application:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesInstanceApplicationsApi->create_instance_application: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_services_instance_applications_use_cases_create_tenant_instance_application_request** | [**EdGraphHttpAggregatorsTenantApiServicesInstanceApplicationsUseCasesCreateTenantInstanceApplicationRequest**](EdGraphHttpAggregatorsTenantApiServicesInstanceApplicationsUseCasesCreateTenantInstanceApplicationRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1InstanceApplicationCreatedResponse**](EdfiAdminApiEdfiAdminV1InstanceApplicationCreatedResponse.md)

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

# **delete_instance_application**
> delete_instance_application(tenant_id, instance_id, application_id)

Deletes an Instance Application

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
    api_instance = edgraph_platform_client.InstancesInstanceApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 'application_id_example' # str | 

    try:
        # Deletes an Instance Application
        api_instance.delete_instance_application(tenant_id, instance_id, application_id)
    except Exception as e:
        print("Exception when calling InstancesInstanceApplicationsApi->delete_instance_application: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **str**|  | 

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

# **get_instance_application_by_id**
> EdfiAdminApiEdfiAdminV1InstanceApplicationProfileResponse get_instance_application_by_id(tenant_id, instance_id, application_id)

Retrieves an Instance Application by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_application_profile_response import EdfiAdminApiEdfiAdminV1InstanceApplicationProfileResponse
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
    api_instance = edgraph_platform_client.InstancesInstanceApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 'application_id_example' # str | 

    try:
        # Retrieves an Instance Application by ID.
        api_response = api_instance.get_instance_application_by_id(tenant_id, instance_id, application_id)
        print("The response of InstancesInstanceApplicationsApi->get_instance_application_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesInstanceApplicationsApi->get_instance_application_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **str**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1InstanceApplicationProfileResponse**](EdfiAdminApiEdfiAdminV1InstanceApplicationProfileResponse.md)

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

# **get_instance_applications**
> EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponsePaginatedItemsViewModel get_instance_applications(tenant_id, instance_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a paginated list of Instance applications

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_applications_list_response_paginated_items_view_model import EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.InstancesInstanceApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a paginated list of Instance applications
        api_response = api_instance.get_instance_applications(tenant_id, instance_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of InstancesInstanceApplicationsApi->get_instance_applications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesInstanceApplicationsApi->get_instance_applications: %s\n" % e)
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

[**EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponsePaginatedItemsViewModel**](EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponsePaginatedItemsViewModel.md)

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

# **update_instance_application**
> EdfiAdminApiEdfiAdminV1InstanceApplicationUpdatedResponse update_instance_application(tenant_id, instance_id, application_id, edfi_admin_api_edfi_admin_v1_update_instance_application_request=edfi_admin_api_edfi_admin_v1_update_instance_application_request)

Updates an Instance Application

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_application_updated_response import EdfiAdminApiEdfiAdminV1InstanceApplicationUpdatedResponse
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_instance_application_request import EdfiAdminApiEdfiAdminV1UpdateInstanceApplicationRequest
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
    api_instance = edgraph_platform_client.InstancesInstanceApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    application_id = 'application_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_update_instance_application_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1UpdateInstanceApplicationRequest() # EdfiAdminApiEdfiAdminV1UpdateInstanceApplicationRequest |  (optional)

    try:
        # Updates an Instance Application
        api_response = api_instance.update_instance_application(tenant_id, instance_id, application_id, edfi_admin_api_edfi_admin_v1_update_instance_application_request=edfi_admin_api_edfi_admin_v1_update_instance_application_request)
        print("The response of InstancesInstanceApplicationsApi->update_instance_application:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesInstanceApplicationsApi->update_instance_application: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **application_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_update_instance_application_request** | [**EdfiAdminApiEdfiAdminV1UpdateInstanceApplicationRequest**](EdfiAdminApiEdfiAdminV1UpdateInstanceApplicationRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1InstanceApplicationUpdatedResponse**](EdfiAdminApiEdfiAdminV1InstanceApplicationUpdatedResponse.md)

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

