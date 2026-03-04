# edgraph_platform_client.SpecificationsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_specification**](SpecificationsApi.md#create_specification) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/specifications | Create a Specification resource
[**delete_specification**](SpecificationsApi.md#delete_specification) | **DELETE** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/specifications/{id} | Delete of Specification resource
[**export_specifications**](SpecificationsApi.md#export_specifications) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/specifications/export | Export all Specifications resources given a Tenant
[**get_specification**](SpecificationsApi.md#get_specification) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/specifications/{id} | Get Specification resource
[**purge_specification**](SpecificationsApi.md#purge_specification) | **DELETE** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/specifications/{specificationId}/purge | Purge a deleted Specification resource
[**recover_specification**](SpecificationsApi.md#recover_specification) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/specifications/{specificationId}/recover | Recover deleted Specification resource
[**search_specifications**](SpecificationsApi.md#search_specifications) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/specifications/search | Seaarch specifications
[**update_specification**](SpecificationsApi.md#update_specification) | **PUT** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/specifications/{id} | Update specification


# **create_specification**
> create_specification(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_create_specification_request=edfi_admin_api_edfi_admin_v1_create_specification_request)

Create a Specification resource

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_specification_request import EdfiAdminApiEdfiAdminV1CreateSpecificationRequest
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
    api_instance = edgraph_platform_client.SpecificationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_create_specification_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1CreateSpecificationRequest() # EdfiAdminApiEdfiAdminV1CreateSpecificationRequest |  (optional)

    try:
        # Create a Specification resource
        api_instance.create_specification(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_create_specification_request=edfi_admin_api_edfi_admin_v1_create_specification_request)
    except Exception as e:
        print("Exception when calling SpecificationsApi->create_specification: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_create_specification_request** | [**EdfiAdminApiEdfiAdminV1CreateSpecificationRequest**](EdfiAdminApiEdfiAdminV1CreateSpecificationRequest.md)|  | [optional] 

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
**400** | Bad Request |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_specification**
> EdfiAdminApiEdfiAdminV1SpecificationDeletedResponse delete_specification(tenant_id, instance_id, id)

Delete of Specification resource

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_specification_deleted_response import EdfiAdminApiEdfiAdminV1SpecificationDeletedResponse
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
    api_instance = edgraph_platform_client.SpecificationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    id = 'id_example' # str | 

    try:
        # Delete of Specification resource
        api_response = api_instance.delete_specification(tenant_id, instance_id, id)
        print("The response of SpecificationsApi->delete_specification:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SpecificationsApi->delete_specification: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **id** | **str**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1SpecificationDeletedResponse**](EdfiAdminApiEdfiAdminV1SpecificationDeletedResponse.md)

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
**200** | Success |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **export_specifications**
> EdfiAdminApiEdfiAdminV1SpecificationsExportedResponse export_specifications(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_export_specifications_request=edfi_admin_api_edfi_admin_v1_export_specifications_request)

Export all Specifications resources given a Tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_export_specifications_request import EdfiAdminApiEdfiAdminV1ExportSpecificationsRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_specifications_exported_response import EdfiAdminApiEdfiAdminV1SpecificationsExportedResponse
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
    api_instance = edgraph_platform_client.SpecificationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_export_specifications_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1ExportSpecificationsRequest() # EdfiAdminApiEdfiAdminV1ExportSpecificationsRequest |  (optional)

    try:
        # Export all Specifications resources given a Tenant
        api_response = api_instance.export_specifications(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_export_specifications_request=edfi_admin_api_edfi_admin_v1_export_specifications_request)
        print("The response of SpecificationsApi->export_specifications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SpecificationsApi->export_specifications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_export_specifications_request** | [**EdfiAdminApiEdfiAdminV1ExportSpecificationsRequest**](EdfiAdminApiEdfiAdminV1ExportSpecificationsRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1SpecificationsExportedResponse**](EdfiAdminApiEdfiAdminV1SpecificationsExportedResponse.md)

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
**400** | Bad Request |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_specification**
> EdfiAdminApiEdfiAdminV1SpecificationResponse get_specification(id, tenant_id, instance_id)

Get Specification resource

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_specification_response import EdfiAdminApiEdfiAdminV1SpecificationResponse
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
    api_instance = edgraph_platform_client.SpecificationsApi(api_client)
    id = 'id_example' # str | 
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 

    try:
        # Get Specification resource
        api_response = api_instance.get_specification(id, tenant_id, instance_id)
        print("The response of SpecificationsApi->get_specification:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SpecificationsApi->get_specification: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1SpecificationResponse**](EdfiAdminApiEdfiAdminV1SpecificationResponse.md)

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
**200** | Success |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **purge_specification**
> EdfiAdminApiEdfiAdminV1SpecificationPurgedResponse purge_specification(tenant_id, instance_id, specification_id)

Purge a deleted Specification resource

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_specification_purged_response import EdfiAdminApiEdfiAdminV1SpecificationPurgedResponse
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
    api_instance = edgraph_platform_client.SpecificationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    specification_id = 'specification_id_example' # str | 

    try:
        # Purge a deleted Specification resource
        api_response = api_instance.purge_specification(tenant_id, instance_id, specification_id)
        print("The response of SpecificationsApi->purge_specification:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SpecificationsApi->purge_specification: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **specification_id** | **str**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1SpecificationPurgedResponse**](EdfiAdminApiEdfiAdminV1SpecificationPurgedResponse.md)

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
**200** | Success |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **recover_specification**
> EdfiAdminApiEdfiAdminV1SpecificationRecoveredResponse recover_specification(tenant_id, instance_id, specification_id)

Recover deleted Specification resource

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_specification_recovered_response import EdfiAdminApiEdfiAdminV1SpecificationRecoveredResponse
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
    api_instance = edgraph_platform_client.SpecificationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    specification_id = 'specification_id_example' # str | 

    try:
        # Recover deleted Specification resource
        api_response = api_instance.recover_specification(tenant_id, instance_id, specification_id)
        print("The response of SpecificationsApi->recover_specification:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SpecificationsApi->recover_specification: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **specification_id** | **str**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1SpecificationRecoveredResponse**](EdfiAdminApiEdfiAdminV1SpecificationRecoveredResponse.md)

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
**200** | Success |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **search_specifications**
> EdfiAdminApiEdfiAdminV1SpecificationsSearchResponse search_specifications(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_search_specifications_request=edfi_admin_api_edfi_admin_v1_search_specifications_request)

Seaarch specifications

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_search_specifications_request import EdfiAdminApiEdfiAdminV1SearchSpecificationsRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_specifications_search_response import EdfiAdminApiEdfiAdminV1SpecificationsSearchResponse
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
    api_instance = edgraph_platform_client.SpecificationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_search_specifications_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1SearchSpecificationsRequest() # EdfiAdminApiEdfiAdminV1SearchSpecificationsRequest |  (optional)

    try:
        # Seaarch specifications
        api_response = api_instance.search_specifications(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_search_specifications_request=edfi_admin_api_edfi_admin_v1_search_specifications_request)
        print("The response of SpecificationsApi->search_specifications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SpecificationsApi->search_specifications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_search_specifications_request** | [**EdfiAdminApiEdfiAdminV1SearchSpecificationsRequest**](EdfiAdminApiEdfiAdminV1SearchSpecificationsRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1SpecificationsSearchResponse**](EdfiAdminApiEdfiAdminV1SpecificationsSearchResponse.md)

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
**400** | Bad Request |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_specification**
> EdfiAdminApiEdfiAdminV1SpecificationUpdatedResponse update_specification(tenant_id, instance_id, id, edfi_admin_api_edfi_admin_v1_update_specification_request=edfi_admin_api_edfi_admin_v1_update_specification_request)

Update specification

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_specification_updated_response import EdfiAdminApiEdfiAdminV1SpecificationUpdatedResponse
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_specification_request import EdfiAdminApiEdfiAdminV1UpdateSpecificationRequest
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
    api_instance = edgraph_platform_client.SpecificationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    id = 'id_example' # str | 
    edfi_admin_api_edfi_admin_v1_update_specification_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1UpdateSpecificationRequest() # EdfiAdminApiEdfiAdminV1UpdateSpecificationRequest |  (optional)

    try:
        # Update specification
        api_response = api_instance.update_specification(tenant_id, instance_id, id, edfi_admin_api_edfi_admin_v1_update_specification_request=edfi_admin_api_edfi_admin_v1_update_specification_request)
        print("The response of SpecificationsApi->update_specification:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SpecificationsApi->update_specification: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_update_specification_request** | [**EdfiAdminApiEdfiAdminV1UpdateSpecificationRequest**](EdfiAdminApiEdfiAdminV1UpdateSpecificationRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1SpecificationUpdatedResponse**](EdfiAdminApiEdfiAdminV1SpecificationUpdatedResponse.md)

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
**400** | Bad Request |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

