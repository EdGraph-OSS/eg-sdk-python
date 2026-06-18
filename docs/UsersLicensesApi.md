# edgraph_platform_client.UsersLicensesApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**assign_license_tenant_user_async**](UsersLicensesApi.md#assign_license_tenant_user_async) | **PUT** /tenants/{tenantId}/users/{userId}/licenses/assign | Assigns a license to a user in the context of a specific tenant
[**assign_license_tenant_user_bulk_async**](UsersLicensesApi.md#assign_license_tenant_user_bulk_async) | **PUT** /tenants/{tenantId}/users/{userId}/licenses/assignbulk | Assigns one or more licenses to a user in the context of a specific tenant
[**get_all_tenant_user_application_licenses_async**](UsersLicensesApi.md#get_all_tenant_user_application_licenses_async) | **GET** /tenants/{tenantId}/users/{userId}/licenses | Retrieves a list of user licenses in the context of a specific tenant
[**revoke_license_tenant_user_async**](UsersLicensesApi.md#revoke_license_tenant_user_async) | **PUT** /tenants/{tenantId}/users/{userId}/licenses/revoke | Revokes a license from a user in the context of a specific tenant
[**revoke_license_tenant_user_bulk_async**](UsersLicensesApi.md#revoke_license_tenant_user_bulk_async) | **PUT** /tenants/{tenantId}/users/{userId}/licenses/revokebulk | Revokes one or more licenses from a user in the context of a specific tenant


# **assign_license_tenant_user_async**
> IdentityApiUserV1LicenseAssignedResponse assign_license_tenant_user_async(tenant_id, user_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_assign_license_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_assign_license_request)

Assigns a license to a user in the context of a specific tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_assign_license_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesAssignLicenseRequest
from edgraph_platform_client.models.identity_api_user_v1_license_assigned_response import IdentityApiUserV1LicenseAssignedResponse
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
    api_instance = edgraph_platform_client.UsersLicensesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    user_id = 'user_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_assign_license_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesAssignLicenseRequest() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesAssignLicenseRequest |  (optional)

    try:
        # Assigns a license to a user in the context of a specific tenant
        api_response = await api_instance.assign_license_tenant_user_async(tenant_id, user_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_assign_license_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_assign_license_request)
        print("The response of UsersLicensesApi->assign_license_tenant_user_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersLicensesApi->assign_license_tenant_user_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **user_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_assign_license_request** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesAssignLicenseRequest**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesAssignLicenseRequest.md)|  | [optional] 

### Return type

[**IdentityApiUserV1LicenseAssignedResponse**](IdentityApiUserV1LicenseAssignedResponse.md)

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

# **assign_license_tenant_user_bulk_async**
> IdentityApiUserV1LicenseAssignedBulkResponse assign_license_tenant_user_bulk_async(tenant_id, user_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_assign_license_bulk_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_assign_license_bulk_request)

Assigns one or more licenses to a user in the context of a specific tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_assign_license_bulk_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesAssignLicenseBulkRequest
from edgraph_platform_client.models.identity_api_user_v1_license_assigned_bulk_response import IdentityApiUserV1LicenseAssignedBulkResponse
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
    api_instance = edgraph_platform_client.UsersLicensesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    user_id = 'user_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_assign_license_bulk_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesAssignLicenseBulkRequest() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesAssignLicenseBulkRequest |  (optional)

    try:
        # Assigns one or more licenses to a user in the context of a specific tenant
        api_response = await api_instance.assign_license_tenant_user_bulk_async(tenant_id, user_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_assign_license_bulk_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_assign_license_bulk_request)
        print("The response of UsersLicensesApi->assign_license_tenant_user_bulk_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersLicensesApi->assign_license_tenant_user_bulk_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **user_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_assign_license_bulk_request** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesAssignLicenseBulkRequest**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesAssignLicenseBulkRequest.md)|  | [optional] 

### Return type

[**IdentityApiUserV1LicenseAssignedBulkResponse**](IdentityApiUserV1LicenseAssignedBulkResponse.md)

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

# **get_all_tenant_user_application_licenses_async**
> EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserLicensePaginatedItemsViewModel get_all_tenant_user_application_licenses_async(tenant_id, user_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of user licenses in the context of a specific tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_license_paginated_items_view_model import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserLicensePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.UsersLicensesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    user_id = 'user_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of user licenses in the context of a specific tenant
        api_response = await api_instance.get_all_tenant_user_application_licenses_async(tenant_id, user_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of UsersLicensesApi->get_all_tenant_user_application_licenses_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersLicensesApi->get_all_tenant_user_application_licenses_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **user_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserLicensePaginatedItemsViewModel**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserLicensePaginatedItemsViewModel.md)

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

# **revoke_license_tenant_user_async**
> IdentityApiUserV1LicenseRevokedResponse revoke_license_tenant_user_async(tenant_id, user_id, identity_api_user_v1_revoke_license_request=identity_api_user_v1_revoke_license_request)

Revokes a license from a user in the context of a specific tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v1_license_revoked_response import IdentityApiUserV1LicenseRevokedResponse
from edgraph_platform_client.models.identity_api_user_v1_revoke_license_request import IdentityApiUserV1RevokeLicenseRequest
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
    api_instance = edgraph_platform_client.UsersLicensesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    user_id = 'user_id_example' # str | 
    identity_api_user_v1_revoke_license_request = edgraph_platform_client.IdentityApiUserV1RevokeLicenseRequest() # IdentityApiUserV1RevokeLicenseRequest |  (optional)

    try:
        # Revokes a license from a user in the context of a specific tenant
        api_response = await api_instance.revoke_license_tenant_user_async(tenant_id, user_id, identity_api_user_v1_revoke_license_request=identity_api_user_v1_revoke_license_request)
        print("The response of UsersLicensesApi->revoke_license_tenant_user_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersLicensesApi->revoke_license_tenant_user_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **user_id** | **str**|  | 
 **identity_api_user_v1_revoke_license_request** | [**IdentityApiUserV1RevokeLicenseRequest**](IdentityApiUserV1RevokeLicenseRequest.md)|  | [optional] 

### Return type

[**IdentityApiUserV1LicenseRevokedResponse**](IdentityApiUserV1LicenseRevokedResponse.md)

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

# **revoke_license_tenant_user_bulk_async**
> IdentityApiUserV1LicenseRevokedBulkResponse revoke_license_tenant_user_bulk_async(tenant_id, user_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_revoke_license_bulk_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_revoke_license_bulk_request)

Revokes one or more licenses from a user in the context of a specific tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_revoke_license_bulk_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesRevokeLicenseBulkRequest
from edgraph_platform_client.models.identity_api_user_v1_license_revoked_bulk_response import IdentityApiUserV1LicenseRevokedBulkResponse
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
    api_instance = edgraph_platform_client.UsersLicensesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    user_id = 'user_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_revoke_license_bulk_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesRevokeLicenseBulkRequest() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesRevokeLicenseBulkRequest |  (optional)

    try:
        # Revokes one or more licenses from a user in the context of a specific tenant
        api_response = await api_instance.revoke_license_tenant_user_bulk_async(tenant_id, user_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_revoke_license_bulk_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_revoke_license_bulk_request)
        print("The response of UsersLicensesApi->revoke_license_tenant_user_bulk_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersLicensesApi->revoke_license_tenant_user_bulk_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **user_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_licenses_revoke_license_bulk_request** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesRevokeLicenseBulkRequest**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesRevokeLicenseBulkRequest.md)|  | [optional] 

### Return type

[**IdentityApiUserV1LicenseRevokedBulkResponse**](IdentityApiUserV1LicenseRevokedBulkResponse.md)

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

