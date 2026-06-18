# edgraph_platform_client.InstancesEducationOrganizationsEducationServiceCentersApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_education_service_center_async**](InstancesEducationOrganizationsEducationServiceCentersApi.md#create_education_service_center_async) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/educationservicecenters | Creates an EducationServiceCenter.
[**delete_education_service_center_async**](InstancesEducationOrganizationsEducationServiceCentersApi.md#delete_education_service_center_async) | **DELETE** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/educationservicecenters/{educationServiceCenterId} | Deletes an EducationServiceCenter.
[**get_education_service_center_by_id_async**](InstancesEducationOrganizationsEducationServiceCentersApi.md#get_education_service_center_by_id_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/educationservicecenters/{educationServiceCenterId} | Retrieves an EducationServiceCenter by ID.
[**update_education_service_center_async**](InstancesEducationOrganizationsEducationServiceCentersApi.md#update_education_service_center_async) | **PUT** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/years/{year}/educationservicecenters/{educationServiceCenterId} | Updates an EducationServiceCenter.


# **create_education_service_center_async**
> EdfiAdminApiEdfiAdminV1EducationServiceCenterCreatedResponse create_education_service_center_async(tenant_id, instance_id, year, edfi_admin_api_edfi_admin_v1_create_education_service_center_request=edfi_admin_api_edfi_admin_v1_create_education_service_center_request)

Creates an EducationServiceCenter.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_education_service_center_request import EdfiAdminApiEdfiAdminV1CreateEducationServiceCenterRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_education_service_center_created_response import EdfiAdminApiEdfiAdminV1EducationServiceCenterCreatedResponse
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
    api_instance = edgraph_platform_client.InstancesEducationOrganizationsEducationServiceCentersApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    edfi_admin_api_edfi_admin_v1_create_education_service_center_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1CreateEducationServiceCenterRequest() # EdfiAdminApiEdfiAdminV1CreateEducationServiceCenterRequest |  (optional)

    try:
        # Creates an EducationServiceCenter.
        api_response = await api_instance.create_education_service_center_async(tenant_id, instance_id, year, edfi_admin_api_edfi_admin_v1_create_education_service_center_request=edfi_admin_api_edfi_admin_v1_create_education_service_center_request)
        print("The response of InstancesEducationOrganizationsEducationServiceCentersApi->create_education_service_center_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesEducationOrganizationsEducationServiceCentersApi->create_education_service_center_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **edfi_admin_api_edfi_admin_v1_create_education_service_center_request** | [**EdfiAdminApiEdfiAdminV1CreateEducationServiceCenterRequest**](EdfiAdminApiEdfiAdminV1CreateEducationServiceCenterRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1EducationServiceCenterCreatedResponse**](EdfiAdminApiEdfiAdminV1EducationServiceCenterCreatedResponse.md)

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

# **delete_education_service_center_async**
> delete_education_service_center_async(tenant_id, instance_id, year, education_service_center_id)

Deletes an EducationServiceCenter.

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
    api_instance = edgraph_platform_client.InstancesEducationOrganizationsEducationServiceCentersApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    education_service_center_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Deletes an EducationServiceCenter.
        await api_instance.delete_education_service_center_async(tenant_id, instance_id, year, education_service_center_id)
    except Exception as e:
        print("Exception when calling InstancesEducationOrganizationsEducationServiceCentersApi->delete_education_service_center_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **education_service_center_id** | **UUID**|  | 

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

# **get_education_service_center_by_id_async**
> EdfiAdminApiEdfiAdminV1EducationServiceCenter get_education_service_center_by_id_async(tenant_id, instance_id, year, education_service_center_id)

Retrieves an EducationServiceCenter by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_education_service_center import EdfiAdminApiEdfiAdminV1EducationServiceCenter
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
    api_instance = edgraph_platform_client.InstancesEducationOrganizationsEducationServiceCentersApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    education_service_center_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Retrieves an EducationServiceCenter by ID.
        api_response = await api_instance.get_education_service_center_by_id_async(tenant_id, instance_id, year, education_service_center_id)
        print("The response of InstancesEducationOrganizationsEducationServiceCentersApi->get_education_service_center_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesEducationOrganizationsEducationServiceCentersApi->get_education_service_center_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **education_service_center_id** | **UUID**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1EducationServiceCenter**](EdfiAdminApiEdfiAdminV1EducationServiceCenter.md)

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

# **update_education_service_center_async**
> update_education_service_center_async(tenant_id, instance_id, year, education_service_center_id, edfi_admin_api_edfi_admin_v1_update_education_service_center_request=edfi_admin_api_edfi_admin_v1_update_education_service_center_request)

Updates an EducationServiceCenter.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_education_service_center_request import EdfiAdminApiEdfiAdminV1UpdateEducationServiceCenterRequest
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
    api_instance = edgraph_platform_client.InstancesEducationOrganizationsEducationServiceCentersApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    instance_id = 'instance_id_example' # str | 
    year = 56 # int | 
    education_service_center_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    edfi_admin_api_edfi_admin_v1_update_education_service_center_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1UpdateEducationServiceCenterRequest() # EdfiAdminApiEdfiAdminV1UpdateEducationServiceCenterRequest |  (optional)

    try:
        # Updates an EducationServiceCenter.
        await api_instance.update_education_service_center_async(tenant_id, instance_id, year, education_service_center_id, edfi_admin_api_edfi_admin_v1_update_education_service_center_request=edfi_admin_api_edfi_admin_v1_update_education_service_center_request)
    except Exception as e:
        print("Exception when calling InstancesEducationOrganizationsEducationServiceCentersApi->update_education_service_center_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **instance_id** | **str**|  | 
 **year** | **int**|  | 
 **education_service_center_id** | **UUID**|  | 
 **edfi_admin_api_edfi_admin_v1_update_education_service_center_request** | [**EdfiAdminApiEdfiAdminV1UpdateEducationServiceCenterRequest**](EdfiAdminApiEdfiAdminV1UpdateEducationServiceCenterRequest.md)|  | [optional] 

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

