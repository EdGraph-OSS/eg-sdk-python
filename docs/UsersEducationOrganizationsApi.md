# edgraph_platform_client.UsersEducationOrganizationsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_user_education_organization**](UsersEducationOrganizationsApi.md#add_user_education_organization) | **POST** /tenants/{tenantId}/users/{userId}/educationorganizations | Adds an Education Organization to a user.
[**get_user_education_organizations**](UsersEducationOrganizationsApi.md#get_user_education_organizations) | **GET** /tenants/{tenantId}/users/{userId}/educationorganizations | Gets the Education Organizations of a user.
[**remove_user_education_organization**](UsersEducationOrganizationsApi.md#remove_user_education_organization) | **DELETE** /tenants/{tenantId}/users/{userId}/educationorganizations/{educationOrganizationId} | Removes an Education Organization from a user.
[**update_user_education_organization**](UsersEducationOrganizationsApi.md#update_user_education_organization) | **PUT** /tenants/{tenantId}/users/{userId}/educationorganizations/{educationOrganizationId} | Updates the Education Organization of a user.


# **add_user_education_organization**
> IdentityApiUserV1EducationOrganizationAddedResponse add_user_education_organization(tenant_id, user_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_education_organizations_add_education_organization_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_education_organizations_add_education_organization_request)

Adds an Education Organization to a user.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_education_organizations_add_education_organization_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEducationOrganizationsAddEducationOrganizationRequest
from edgraph_platform_client.models.identity_api_user_v1_education_organization_added_response import IdentityApiUserV1EducationOrganizationAddedResponse
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
    api_instance = edgraph_platform_client.UsersEducationOrganizationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    user_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_education_organizations_add_education_organization_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEducationOrganizationsAddEducationOrganizationRequest() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEducationOrganizationsAddEducationOrganizationRequest |  (optional)

    try:
        # Adds an Education Organization to a user.
        api_response = await api_instance.add_user_education_organization(tenant_id, user_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_education_organizations_add_education_organization_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_education_organizations_add_education_organization_request)
        print("The response of UsersEducationOrganizationsApi->add_user_education_organization:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersEducationOrganizationsApi->add_user_education_organization: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **user_id** | **UUID**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_education_organizations_add_education_organization_request** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEducationOrganizationsAddEducationOrganizationRequest**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEducationOrganizationsAddEducationOrganizationRequest.md)|  | [optional] 

### Return type

[**IdentityApiUserV1EducationOrganizationAddedResponse**](IdentityApiUserV1EducationOrganizationAddedResponse.md)

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

# **get_user_education_organizations**
> IdentityApiUserV1EducationOrganizationPaginatedItemsResponse get_user_education_organizations(tenant_id, user_id)

Gets the Education Organizations of a user.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v1_education_organization_paginated_items_response import IdentityApiUserV1EducationOrganizationPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.UsersEducationOrganizationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    user_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets the Education Organizations of a user.
        api_response = await api_instance.get_user_education_organizations(tenant_id, user_id)
        print("The response of UsersEducationOrganizationsApi->get_user_education_organizations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersEducationOrganizationsApi->get_user_education_organizations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **user_id** | **UUID**|  | 

### Return type

[**IdentityApiUserV1EducationOrganizationPaginatedItemsResponse**](IdentityApiUserV1EducationOrganizationPaginatedItemsResponse.md)

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

# **remove_user_education_organization**
> IdentityApiUserV1EducationOrganizationRemovedResponse remove_user_education_organization(tenant_id, user_id, education_organization_id)

Removes an Education Organization from a user.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v1_education_organization_removed_response import IdentityApiUserV1EducationOrganizationRemovedResponse
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
    api_instance = edgraph_platform_client.UsersEducationOrganizationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    user_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    education_organization_id = 56 # int | 

    try:
        # Removes an Education Organization from a user.
        api_response = await api_instance.remove_user_education_organization(tenant_id, user_id, education_organization_id)
        print("The response of UsersEducationOrganizationsApi->remove_user_education_organization:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersEducationOrganizationsApi->remove_user_education_organization: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **user_id** | **UUID**|  | 
 **education_organization_id** | **int**|  | 

### Return type

[**IdentityApiUserV1EducationOrganizationRemovedResponse**](IdentityApiUserV1EducationOrganizationRemovedResponse.md)

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

# **update_user_education_organization**
> IdentityApiUserV1EducationOrganizationUpdatedResponse update_user_education_organization(tenant_id, user_id, education_organization_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_education_organizations_update_education_organization_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_education_organizations_update_education_organization_request)

Updates the Education Organization of a user.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_education_organizations_update_education_organization_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEducationOrganizationsUpdateEducationOrganizationRequest
from edgraph_platform_client.models.identity_api_user_v1_education_organization_updated_response import IdentityApiUserV1EducationOrganizationUpdatedResponse
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
    api_instance = edgraph_platform_client.UsersEducationOrganizationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    user_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    education_organization_id = 56 # int | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_education_organizations_update_education_organization_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEducationOrganizationsUpdateEducationOrganizationRequest() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEducationOrganizationsUpdateEducationOrganizationRequest |  (optional)

    try:
        # Updates the Education Organization of a user.
        api_response = await api_instance.update_user_education_organization(tenant_id, user_id, education_organization_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_education_organizations_update_education_organization_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_education_organizations_update_education_organization_request)
        print("The response of UsersEducationOrganizationsApi->update_user_education_organization:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersEducationOrganizationsApi->update_user_education_organization: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **user_id** | **UUID**|  | 
 **education_organization_id** | **int**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_education_organizations_update_education_organization_request** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEducationOrganizationsUpdateEducationOrganizationRequest**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEducationOrganizationsUpdateEducationOrganizationRequest.md)|  | [optional] 

### Return type

[**IdentityApiUserV1EducationOrganizationUpdatedResponse**](IdentityApiUserV1EducationOrganizationUpdatedResponse.md)

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

