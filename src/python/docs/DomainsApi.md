# edgraph_platform_client.DomainsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_tenant_domain_async**](DomainsApi.md#create_tenant_domain_async) | **POST** /tenants/{tenantId}/domains | Creates a new domain
[**delete_tenant_domain_async**](DomainsApi.md#delete_tenant_domain_async) | **DELETE** /tenants/{tenantId}/domains/{domainName} | Deletes a user
[**get_all_tenant_domains_async**](DomainsApi.md#get_all_tenant_domains_async) | **GET** /tenants/{tenantId}/domains | Retrieves a list of domains associated to this tenant
[**get_tenant_domain_profile_by_name_async**](DomainsApi.md#get_tenant_domain_profile_by_name_async) | **GET** /tenants/{tenantId}/domains/{domainName} | Retrieves a domain
[**update_tenant_domain_async**](DomainsApi.md#update_tenant_domain_async) | **PUT** /tenants/{tenantId}/domains/{domainName} | Updates a domain
[**verify_tenant_domain_async**](DomainsApi.md#verify_tenant_domain_async) | **PUT** /tenants/{tenantId}/domains/{domainName}/verify | Verify a  tenant&#39;s domain


# **create_tenant_domain_async**
> TenantApiTenantV1DomainCreatedResponse create_tenant_domain_async(tenant_id, tenant_api_tenant_v1_create_domain_request=tenant_api_tenant_v1_create_domain_request)

Creates a new domain

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_tenant_v1_create_domain_request import TenantApiTenantV1CreateDomainRequest
from edgraph_platform_client.models.tenant_api_tenant_v1_domain_created_response import TenantApiTenantV1DomainCreatedResponse
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
    api_instance = edgraph_platform_client.DomainsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    tenant_api_tenant_v1_create_domain_request = edgraph_platform_client.TenantApiTenantV1CreateDomainRequest() # TenantApiTenantV1CreateDomainRequest |  (optional)

    try:
        # Creates a new domain
        api_response = api_instance.create_tenant_domain_async(tenant_id, tenant_api_tenant_v1_create_domain_request=tenant_api_tenant_v1_create_domain_request)
        print("The response of DomainsApi->create_tenant_domain_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DomainsApi->create_tenant_domain_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **tenant_api_tenant_v1_create_domain_request** | [**TenantApiTenantV1CreateDomainRequest**](TenantApiTenantV1CreateDomainRequest.md)|  | [optional] 

### Return type

[**TenantApiTenantV1DomainCreatedResponse**](TenantApiTenantV1DomainCreatedResponse.md)

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

# **delete_tenant_domain_async**
> delete_tenant_domain_async(tenant_id, domain_name)

Deletes a user

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
    api_instance = edgraph_platform_client.DomainsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    domain_name = 'domain_name_example' # str | 

    try:
        # Deletes a user
        api_instance.delete_tenant_domain_async(tenant_id, domain_name)
    except Exception as e:
        print("Exception when calling DomainsApi->delete_tenant_domain_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **domain_name** | **str**|  | 

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_all_tenant_domains_async**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesDomainListResponseDtoPaginatedItemsViewModel get_all_tenant_domains_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of domains associated to this tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_domain_list_response_dto_paginated_items_view_model import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesDomainListResponseDtoPaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.DomainsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of domains associated to this tenant
        api_response = api_instance.get_all_tenant_domains_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of DomainsApi->get_all_tenant_domains_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DomainsApi->get_all_tenant_domains_async: %s\n" % e)
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

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesDomainListResponseDtoPaginatedItemsViewModel**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesDomainListResponseDtoPaginatedItemsViewModel.md)

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

# **get_tenant_domain_profile_by_name_async**
> TenantApiTenantV1DomainProfileResponse get_tenant_domain_profile_by_name_async(tenant_id, domain_name)

Retrieves a domain

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_tenant_v1_domain_profile_response import TenantApiTenantV1DomainProfileResponse
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
    api_instance = edgraph_platform_client.DomainsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    domain_name = 'domain_name_example' # str | 

    try:
        # Retrieves a domain
        api_response = api_instance.get_tenant_domain_profile_by_name_async(tenant_id, domain_name)
        print("The response of DomainsApi->get_tenant_domain_profile_by_name_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DomainsApi->get_tenant_domain_profile_by_name_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **domain_name** | **str**|  | 

### Return type

[**TenantApiTenantV1DomainProfileResponse**](TenantApiTenantV1DomainProfileResponse.md)

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

# **update_tenant_domain_async**
> TenantApiTenantV1DomainUpdatedResponse update_tenant_domain_async(tenant_id, domain_name, tenant_api_tenant_v1_update_domain_request=tenant_api_tenant_v1_update_domain_request)

Updates a domain

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_tenant_v1_domain_updated_response import TenantApiTenantV1DomainUpdatedResponse
from edgraph_platform_client.models.tenant_api_tenant_v1_update_domain_request import TenantApiTenantV1UpdateDomainRequest
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
    api_instance = edgraph_platform_client.DomainsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    domain_name = 'domain_name_example' # str | 
    tenant_api_tenant_v1_update_domain_request = edgraph_platform_client.TenantApiTenantV1UpdateDomainRequest() # TenantApiTenantV1UpdateDomainRequest |  (optional)

    try:
        # Updates a domain
        api_response = api_instance.update_tenant_domain_async(tenant_id, domain_name, tenant_api_tenant_v1_update_domain_request=tenant_api_tenant_v1_update_domain_request)
        print("The response of DomainsApi->update_tenant_domain_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DomainsApi->update_tenant_domain_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **domain_name** | **str**|  | 
 **tenant_api_tenant_v1_update_domain_request** | [**TenantApiTenantV1UpdateDomainRequest**](TenantApiTenantV1UpdateDomainRequest.md)|  | [optional] 

### Return type

[**TenantApiTenantV1DomainUpdatedResponse**](TenantApiTenantV1DomainUpdatedResponse.md)

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

# **verify_tenant_domain_async**
> TenantApiTenantV1DomainVerifiedResponse verify_tenant_domain_async(tenant_id, domain_name, tenant_api_tenant_v1_verify_domain_request=tenant_api_tenant_v1_verify_domain_request)

Verify a  tenant's domain

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_tenant_v1_domain_verified_response import TenantApiTenantV1DomainVerifiedResponse
from edgraph_platform_client.models.tenant_api_tenant_v1_verify_domain_request import TenantApiTenantV1VerifyDomainRequest
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
    api_instance = edgraph_platform_client.DomainsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    domain_name = 'domain_name_example' # str | 
    tenant_api_tenant_v1_verify_domain_request = edgraph_platform_client.TenantApiTenantV1VerifyDomainRequest() # TenantApiTenantV1VerifyDomainRequest |  (optional)

    try:
        # Verify a  tenant's domain
        api_response = api_instance.verify_tenant_domain_async(tenant_id, domain_name, tenant_api_tenant_v1_verify_domain_request=tenant_api_tenant_v1_verify_domain_request)
        print("The response of DomainsApi->verify_tenant_domain_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DomainsApi->verify_tenant_domain_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **domain_name** | **str**|  | 
 **tenant_api_tenant_v1_verify_domain_request** | [**TenantApiTenantV1VerifyDomainRequest**](TenantApiTenantV1VerifyDomainRequest.md)|  | [optional] 

### Return type

[**TenantApiTenantV1DomainVerifiedResponse**](TenantApiTenantV1DomainVerifiedResponse.md)

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

