# edgraph_platform_client.InstancesClaimSetsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_claim_set_async**](InstancesClaimSetsApi.md#create_claim_set_async) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/claimsets | Creates a ClaimSet.
[**delete_claim_set_async**](InstancesClaimSetsApi.md#delete_claim_set_async) | **DELETE** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/claimsets/{claimSetId} | Deletes a ClaimSet.
[**get_claim_set_by_id_async**](InstancesClaimSetsApi.md#get_claim_set_by_id_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/claimsets/{claimSetId} | Retrieves a ClaimSet by ID.
[**get_claim_sets_async**](InstancesClaimSetsApi.md#get_claim_sets_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/claimsets | Retrieves a list of ClaimSets.
[**get_resource_claims_grid_async**](InstancesClaimSetsApi.md#get_resource_claims_grid_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/claimsets/{claimSetId}/resourceclaims | Retrieves a grid of Resource Claims.
[**sync_claim_set_async**](InstancesClaimSetsApi.md#sync_claim_set_async) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/claimsets/{claimSetId}/sync | Copies a Claim Set from one instance to another/other instance(s)
[**update_claim_set_async**](InstancesClaimSetsApi.md#update_claim_set_async) | **PUT** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/claimsets/{claimSetId} | Updates a ClaimSet.


# **create_claim_set_async**
> EdfiAdminApiEdfiAdminV1SaveClaimSetResponse create_claim_set_async(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_save_claim_set_request=edfi_admin_api_edfi_admin_v1_save_claim_set_request)

Creates a ClaimSet.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_save_claim_set_request import EdfiAdminApiEdfiAdminV1SaveClaimSetRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_save_claim_set_response import EdfiAdminApiEdfiAdminV1SaveClaimSetResponse
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
    api_instance = edgraph_platform_client.InstancesClaimSetsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_save_claim_set_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1SaveClaimSetRequest() # EdfiAdminApiEdfiAdminV1SaveClaimSetRequest |  (optional)

    try:
        # Creates a ClaimSet.
        api_response = api_instance.create_claim_set_async(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_save_claim_set_request=edfi_admin_api_edfi_admin_v1_save_claim_set_request)
        print("The response of InstancesClaimSetsApi->create_claim_set_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesClaimSetsApi->create_claim_set_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_save_claim_set_request** | [**EdfiAdminApiEdfiAdminV1SaveClaimSetRequest**](EdfiAdminApiEdfiAdminV1SaveClaimSetRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1SaveClaimSetResponse**](EdfiAdminApiEdfiAdminV1SaveClaimSetResponse.md)

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

# **delete_claim_set_async**
> delete_claim_set_async(tenant_id, instance_id, claim_set_id)

Deletes a ClaimSet.

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
    api_instance = edgraph_platform_client.InstancesClaimSetsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    claim_set_id = 56 # int | 

    try:
        # Deletes a ClaimSet.
        api_instance.delete_claim_set_async(tenant_id, instance_id, claim_set_id)
    except Exception as e:
        print("Exception when calling InstancesClaimSetsApi->delete_claim_set_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **claim_set_id** | **int**|  | 

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

# **get_claim_set_by_id_async**
> EdfiAdminApiEdfiAdminV1ClaimSet get_claim_set_by_id_async(tenant_id, instance_id, claim_set_id)

Retrieves a ClaimSet by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_claim_set import EdfiAdminApiEdfiAdminV1ClaimSet
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
    api_instance = edgraph_platform_client.InstancesClaimSetsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    claim_set_id = 56 # int | 

    try:
        # Retrieves a ClaimSet by ID.
        api_response = api_instance.get_claim_set_by_id_async(tenant_id, instance_id, claim_set_id)
        print("The response of InstancesClaimSetsApi->get_claim_set_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesClaimSetsApi->get_claim_set_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **claim_set_id** | **int**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1ClaimSet**](EdfiAdminApiEdfiAdminV1ClaimSet.md)

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

# **get_claim_sets_async**
> EdfiAdminApiEdfiAdminV1ClaimSetPaginatedItemsViewModel get_claim_sets_async(tenant_id, instance_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of ClaimSets.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_claim_set_paginated_items_view_model import EdfiAdminApiEdfiAdminV1ClaimSetPaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.InstancesClaimSetsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of ClaimSets.
        api_response = api_instance.get_claim_sets_async(tenant_id, instance_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of InstancesClaimSetsApi->get_claim_sets_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesClaimSetsApi->get_claim_sets_async: %s\n" % e)
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

[**EdfiAdminApiEdfiAdminV1ClaimSetPaginatedItemsViewModel**](EdfiAdminApiEdfiAdminV1ClaimSetPaginatedItemsViewModel.md)

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

# **get_resource_claims_grid_async**
> EdfiAdminApiEdfiAdminV1GetResourceClaimsGridResponse get_resource_claims_grid_async(tenant_id, instance_id, claim_set_id)

Retrieves a grid of Resource Claims.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_get_resource_claims_grid_response import EdfiAdminApiEdfiAdminV1GetResourceClaimsGridResponse
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
    api_instance = edgraph_platform_client.InstancesClaimSetsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    claim_set_id = 56 # int | 

    try:
        # Retrieves a grid of Resource Claims.
        api_response = api_instance.get_resource_claims_grid_async(tenant_id, instance_id, claim_set_id)
        print("The response of InstancesClaimSetsApi->get_resource_claims_grid_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesClaimSetsApi->get_resource_claims_grid_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **claim_set_id** | **int**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1GetResourceClaimsGridResponse**](EdfiAdminApiEdfiAdminV1GetResourceClaimsGridResponse.md)

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

# **sync_claim_set_async**
> sync_claim_set_async(tenant_id, instance_id, claim_set_id, edfi_admin_api_edfi_admin_v1_sync_claim_set_request=edfi_admin_api_edfi_admin_v1_sync_claim_set_request)

Copies a Claim Set from one instance to another/other instance(s)

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_sync_claim_set_request import EdfiAdminApiEdfiAdminV1SyncClaimSetRequest
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
    api_instance = edgraph_platform_client.InstancesClaimSetsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    claim_set_id = 56 # int | 
    edfi_admin_api_edfi_admin_v1_sync_claim_set_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1SyncClaimSetRequest() # EdfiAdminApiEdfiAdminV1SyncClaimSetRequest |  (optional)

    try:
        # Copies a Claim Set from one instance to another/other instance(s)
        api_instance.sync_claim_set_async(tenant_id, instance_id, claim_set_id, edfi_admin_api_edfi_admin_v1_sync_claim_set_request=edfi_admin_api_edfi_admin_v1_sync_claim_set_request)
    except Exception as e:
        print("Exception when calling InstancesClaimSetsApi->sync_claim_set_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **claim_set_id** | **int**|  | 
 **edfi_admin_api_edfi_admin_v1_sync_claim_set_request** | [**EdfiAdminApiEdfiAdminV1SyncClaimSetRequest**](EdfiAdminApiEdfiAdminV1SyncClaimSetRequest.md)|  | [optional] 

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

# **update_claim_set_async**
> EdfiAdminApiEdfiAdminV1SaveClaimSetResponse update_claim_set_async(tenant_id, instance_id, claim_set_id, edfi_admin_api_edfi_admin_v1_save_claim_set_request=edfi_admin_api_edfi_admin_v1_save_claim_set_request)

Updates a ClaimSet.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_save_claim_set_request import EdfiAdminApiEdfiAdminV1SaveClaimSetRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_save_claim_set_response import EdfiAdminApiEdfiAdminV1SaveClaimSetResponse
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
    api_instance = edgraph_platform_client.InstancesClaimSetsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    claim_set_id = 56 # int | 
    edfi_admin_api_edfi_admin_v1_save_claim_set_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1SaveClaimSetRequest() # EdfiAdminApiEdfiAdminV1SaveClaimSetRequest |  (optional)

    try:
        # Updates a ClaimSet.
        api_response = api_instance.update_claim_set_async(tenant_id, instance_id, claim_set_id, edfi_admin_api_edfi_admin_v1_save_claim_set_request=edfi_admin_api_edfi_admin_v1_save_claim_set_request)
        print("The response of InstancesClaimSetsApi->update_claim_set_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesClaimSetsApi->update_claim_set_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **claim_set_id** | **int**|  | 
 **edfi_admin_api_edfi_admin_v1_save_claim_set_request** | [**EdfiAdminApiEdfiAdminV1SaveClaimSetRequest**](EdfiAdminApiEdfiAdminV1SaveClaimSetRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1SaveClaimSetResponse**](EdfiAdminApiEdfiAdminV1SaveClaimSetResponse.md)

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

