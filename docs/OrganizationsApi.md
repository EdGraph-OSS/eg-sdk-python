# edgraph_platform_client.OrganizationsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_organization_async**](OrganizationsApi.md#create_organization_async) | **POST** /tenants/{tenantId}/organizations | Creates an Organization.
[**delete_organization_async**](OrganizationsApi.md#delete_organization_async) | **DELETE** /tenants/{tenantId}/organizations/{organizationIdentifier} | Deletes an Organization.
[**get_organization_by_id_async**](OrganizationsApi.md#get_organization_by_id_async) | **GET** /tenants/{tenantId}/organizations/{organizationIdentifier} | Retrieves an Organization by ID.
[**get_organizations_async**](OrganizationsApi.md#get_organizations_async) | **GET** /tenants/{tenantId}/organizations | Retrieves a list of Organizations.
[**update_organization_async**](OrganizationsApi.md#update_organization_async) | **PUT** /tenants/{tenantId}/organizations/{organizationIdentifier} | Updates an Organization.


# **create_organization_async**
> TenantApiTenantV1OrganizationCreatedResponse create_organization_async(tenant_id, tenant_api_tenant_v1_create_organization_request=tenant_api_tenant_v1_create_organization_request)

Creates an Organization.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_tenant_v1_create_organization_request import TenantApiTenantV1CreateOrganizationRequest
from edgraph_platform_client.models.tenant_api_tenant_v1_organization_created_response import TenantApiTenantV1OrganizationCreatedResponse
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
    api_instance = edgraph_platform_client.OrganizationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    tenant_api_tenant_v1_create_organization_request = edgraph_platform_client.TenantApiTenantV1CreateOrganizationRequest() # TenantApiTenantV1CreateOrganizationRequest |  (optional)

    try:
        # Creates an Organization.
        api_response = api_instance.create_organization_async(tenant_id, tenant_api_tenant_v1_create_organization_request=tenant_api_tenant_v1_create_organization_request)
        print("The response of OrganizationsApi->create_organization_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganizationsApi->create_organization_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **tenant_api_tenant_v1_create_organization_request** | [**TenantApiTenantV1CreateOrganizationRequest**](TenantApiTenantV1CreateOrganizationRequest.md)|  | [optional] 

### Return type

[**TenantApiTenantV1OrganizationCreatedResponse**](TenantApiTenantV1OrganizationCreatedResponse.md)

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

# **delete_organization_async**
> TenantApiTenantV1OrganizationDeletedResponse delete_organization_async(tenant_id, organization_identifier)

Deletes an Organization.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_tenant_v1_organization_deleted_response import TenantApiTenantV1OrganizationDeletedResponse
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
    api_instance = edgraph_platform_client.OrganizationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    organization_identifier = 'organization_identifier_example' # str | 

    try:
        # Deletes an Organization.
        api_response = api_instance.delete_organization_async(tenant_id, organization_identifier)
        print("The response of OrganizationsApi->delete_organization_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganizationsApi->delete_organization_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **organization_identifier** | **str**|  | 

### Return type

[**TenantApiTenantV1OrganizationDeletedResponse**](TenantApiTenantV1OrganizationDeletedResponse.md)

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

# **get_organization_by_id_async**
> TenantApiTenantV1Organization get_organization_by_id_async(tenant_id, organization_identifier)

Retrieves an Organization by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_tenant_v1_organization import TenantApiTenantV1Organization
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
    api_instance = edgraph_platform_client.OrganizationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    organization_identifier = 'organization_identifier_example' # str | 

    try:
        # Retrieves an Organization by ID.
        api_response = api_instance.get_organization_by_id_async(tenant_id, organization_identifier)
        print("The response of OrganizationsApi->get_organization_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganizationsApi->get_organization_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **organization_identifier** | **str**|  | 

### Return type

[**TenantApiTenantV1Organization**](TenantApiTenantV1Organization.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_organizations_async**
> TenantApiTenantV1GetOrganizationsPaginatedResponse get_organizations_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of Organizations.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_tenant_v1_get_organizations_paginated_response import TenantApiTenantV1GetOrganizationsPaginatedResponse
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
    api_instance = edgraph_platform_client.OrganizationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of Organizations.
        api_response = api_instance.get_organizations_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of OrganizationsApi->get_organizations_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganizationsApi->get_organizations_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**TenantApiTenantV1GetOrganizationsPaginatedResponse**](TenantApiTenantV1GetOrganizationsPaginatedResponse.md)

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

# **update_organization_async**
> TenantApiTenantV1OrganizationUpdatedResponse update_organization_async(tenant_id, organization_identifier, tenant_api_tenant_v1_update_organization_request=tenant_api_tenant_v1_update_organization_request)

Updates an Organization.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_tenant_v1_organization_updated_response import TenantApiTenantV1OrganizationUpdatedResponse
from edgraph_platform_client.models.tenant_api_tenant_v1_update_organization_request import TenantApiTenantV1UpdateOrganizationRequest
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
    api_instance = edgraph_platform_client.OrganizationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    organization_identifier = 'organization_identifier_example' # str | 
    tenant_api_tenant_v1_update_organization_request = edgraph_platform_client.TenantApiTenantV1UpdateOrganizationRequest() # TenantApiTenantV1UpdateOrganizationRequest |  (optional)

    try:
        # Updates an Organization.
        api_response = api_instance.update_organization_async(tenant_id, organization_identifier, tenant_api_tenant_v1_update_organization_request=tenant_api_tenant_v1_update_organization_request)
        print("The response of OrganizationsApi->update_organization_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganizationsApi->update_organization_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **organization_identifier** | **str**|  | 
 **tenant_api_tenant_v1_update_organization_request** | [**TenantApiTenantV1UpdateOrganizationRequest**](TenantApiTenantV1UpdateOrganizationRequest.md)|  | [optional] 

### Return type

[**TenantApiTenantV1OrganizationUpdatedResponse**](TenantApiTenantV1OrganizationUpdatedResponse.md)

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

