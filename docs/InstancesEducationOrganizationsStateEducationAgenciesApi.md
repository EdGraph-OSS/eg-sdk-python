# edgraph_platform_client.InstancesEducationOrganizationsStateEducationAgenciesApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_state_education_agency_async**](InstancesEducationOrganizationsStateEducationAgenciesApi.md#create_state_education_agency_async) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/stateeducationagencies | Creates a StateEducationAgency.
[**delete_state_education_agency_async**](InstancesEducationOrganizationsStateEducationAgenciesApi.md#delete_state_education_agency_async) | **DELETE** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/stateeducationagencies/{stateEducationAgencyId} | Deletes a StateEducationAgency.
[**get_state_education_agency_by_id_async**](InstancesEducationOrganizationsStateEducationAgenciesApi.md#get_state_education_agency_by_id_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/stateeducationagencies/{stateEducationAgencyId} | Retrieves a StateEducationAgency by ID.
[**update_state_education_agency_async**](InstancesEducationOrganizationsStateEducationAgenciesApi.md#update_state_education_agency_async) | **PUT** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/stateeducationagencies/{stateEducationAgencyId} | Updates a StateEducationAgency.


# **create_state_education_agency_async**
> EdfiAdminApiEdfiAdminV1StateEducationAgencyCreatedResponse create_state_education_agency_async(tenant_id, instance_id, year, edfi_admin_api_edfi_admin_v1_create_state_education_agency_request=edfi_admin_api_edfi_admin_v1_create_state_education_agency_request)

Creates a StateEducationAgency.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_state_education_agency_request import EdfiAdminApiEdfiAdminV1CreateStateEducationAgencyRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_state_education_agency_created_response import EdfiAdminApiEdfiAdminV1StateEducationAgencyCreatedResponse
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
    api_instance = edgraph_platform_client.InstancesEducationOrganizationsStateEducationAgenciesApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    edfi_admin_api_edfi_admin_v1_create_state_education_agency_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1CreateStateEducationAgencyRequest() # EdfiAdminApiEdfiAdminV1CreateStateEducationAgencyRequest |  (optional)

    try:
        # Creates a StateEducationAgency.
        api_response = await api_instance.create_state_education_agency_async(tenant_id, instance_id, year, edfi_admin_api_edfi_admin_v1_create_state_education_agency_request=edfi_admin_api_edfi_admin_v1_create_state_education_agency_request)
        print("The response of InstancesEducationOrganizationsStateEducationAgenciesApi->create_state_education_agency_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesEducationOrganizationsStateEducationAgenciesApi->create_state_education_agency_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **edfi_admin_api_edfi_admin_v1_create_state_education_agency_request** | [**EdfiAdminApiEdfiAdminV1CreateStateEducationAgencyRequest**](EdfiAdminApiEdfiAdminV1CreateStateEducationAgencyRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1StateEducationAgencyCreatedResponse**](EdfiAdminApiEdfiAdminV1StateEducationAgencyCreatedResponse.md)

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

# **delete_state_education_agency_async**
> delete_state_education_agency_async(tenant_id, instance_id, year, state_education_agency_id)

Deletes a StateEducationAgency.

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
    api_instance = edgraph_platform_client.InstancesEducationOrganizationsStateEducationAgenciesApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    state_education_agency_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Deletes a StateEducationAgency.
        await api_instance.delete_state_education_agency_async(tenant_id, instance_id, year, state_education_agency_id)
    except Exception as e:
        print("Exception when calling InstancesEducationOrganizationsStateEducationAgenciesApi->delete_state_education_agency_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **state_education_agency_id** | **UUID**|  | 

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

# **get_state_education_agency_by_id_async**
> EdfiAdminApiEdfiAdminV1StateEducationAgency get_state_education_agency_by_id_async(tenant_id, instance_id, year, state_education_agency_id)

Retrieves a StateEducationAgency by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_state_education_agency import EdfiAdminApiEdfiAdminV1StateEducationAgency
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
    api_instance = edgraph_platform_client.InstancesEducationOrganizationsStateEducationAgenciesApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    state_education_agency_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Retrieves a StateEducationAgency by ID.
        api_response = await api_instance.get_state_education_agency_by_id_async(tenant_id, instance_id, year, state_education_agency_id)
        print("The response of InstancesEducationOrganizationsStateEducationAgenciesApi->get_state_education_agency_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesEducationOrganizationsStateEducationAgenciesApi->get_state_education_agency_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **state_education_agency_id** | **UUID**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1StateEducationAgency**](EdfiAdminApiEdfiAdminV1StateEducationAgency.md)

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

# **update_state_education_agency_async**
> update_state_education_agency_async(tenant_id, instance_id, year, state_education_agency_id, edfi_admin_api_edfi_admin_v1_update_state_education_agency_request=edfi_admin_api_edfi_admin_v1_update_state_education_agency_request)

Updates a StateEducationAgency.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_state_education_agency_request import EdfiAdminApiEdfiAdminV1UpdateStateEducationAgencyRequest
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
    api_instance = edgraph_platform_client.InstancesEducationOrganizationsStateEducationAgenciesApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    state_education_agency_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    edfi_admin_api_edfi_admin_v1_update_state_education_agency_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1UpdateStateEducationAgencyRequest() # EdfiAdminApiEdfiAdminV1UpdateStateEducationAgencyRequest |  (optional)

    try:
        # Updates a StateEducationAgency.
        await api_instance.update_state_education_agency_async(tenant_id, instance_id, year, state_education_agency_id, edfi_admin_api_edfi_admin_v1_update_state_education_agency_request=edfi_admin_api_edfi_admin_v1_update_state_education_agency_request)
    except Exception as e:
        print("Exception when calling InstancesEducationOrganizationsStateEducationAgenciesApi->update_state_education_agency_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **state_education_agency_id** | **UUID**|  | 
 **edfi_admin_api_edfi_admin_v1_update_state_education_agency_request** | [**EdfiAdminApiEdfiAdminV1UpdateStateEducationAgencyRequest**](EdfiAdminApiEdfiAdminV1UpdateStateEducationAgencyRequest.md)|  | [optional] 

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

