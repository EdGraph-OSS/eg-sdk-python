# edgraph_platform_client.UsersSectionsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_user_section**](UsersSectionsApi.md#add_user_section) | **POST** /tenants/{tenantId}/users/{userId}/sections | Adds a Section to a user.
[**add_user_section_bulk**](UsersSectionsApi.md#add_user_section_bulk) | **POST** /tenants/{tenantId}/users/{userId}/sections/bulk | Adds Sections to a user in bulk.
[**get_user_sections**](UsersSectionsApi.md#get_user_sections) | **GET** /tenants/{tenantId}/users/{userId}/sections | Gets the Sections of a user.
[**remove_user_section**](UsersSectionsApi.md#remove_user_section) | **DELETE** /tenants/{tenantId}/users/{userId}/sections/{userSectionId} | Removes a Section from a user.
[**remove_user_section_bulk**](UsersSectionsApi.md#remove_user_section_bulk) | **DELETE** /tenants/{tenantId}/users/{userId}/sections/bulk | Removes Sections from a user in bulk.
[**update_user_section**](UsersSectionsApi.md#update_user_section) | **PUT** /tenants/{tenantId}/users/{userId}/sections/{userSectionId} | Updates the Section of a user.
[**update_user_section_bulk**](UsersSectionsApi.md#update_user_section_bulk) | **PUT** /tenants/{tenantId}/users/{userId}/sections/bulk | Updates the Section of a user in bulk.


# **add_user_section**
> IdentityApiUserV1SectionAddedResponse add_user_section(tenant_id, user_id, identity_api_user_v1_add_section_request=identity_api_user_v1_add_section_request)

Adds a Section to a user.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v1_add_section_request import IdentityApiUserV1AddSectionRequest
from edgraph_platform_client.models.identity_api_user_v1_section_added_response import IdentityApiUserV1SectionAddedResponse
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
    api_instance = edgraph_platform_client.UsersSectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    user_id = 'user_id_example' # str | 
    identity_api_user_v1_add_section_request = edgraph_platform_client.IdentityApiUserV1AddSectionRequest() # IdentityApiUserV1AddSectionRequest |  (optional)

    try:
        # Adds a Section to a user.
        api_response = api_instance.add_user_section(tenant_id, user_id, identity_api_user_v1_add_section_request=identity_api_user_v1_add_section_request)
        print("The response of UsersSectionsApi->add_user_section:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersSectionsApi->add_user_section: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **user_id** | **str**|  | 
 **identity_api_user_v1_add_section_request** | [**IdentityApiUserV1AddSectionRequest**](IdentityApiUserV1AddSectionRequest.md)|  | [optional] 

### Return type

[**IdentityApiUserV1SectionAddedResponse**](IdentityApiUserV1SectionAddedResponse.md)

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

# **add_user_section_bulk**
> IdentityApiUserV1SectionAddedBulkResponse add_user_section_bulk(tenant_id, user_id, identity_api_user_v1_add_section_bulk_request=identity_api_user_v1_add_section_bulk_request)

Adds Sections to a user in bulk.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v1_add_section_bulk_request import IdentityApiUserV1AddSectionBulkRequest
from edgraph_platform_client.models.identity_api_user_v1_section_added_bulk_response import IdentityApiUserV1SectionAddedBulkResponse
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
    api_instance = edgraph_platform_client.UsersSectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    user_id = 'user_id_example' # str | 
    identity_api_user_v1_add_section_bulk_request = edgraph_platform_client.IdentityApiUserV1AddSectionBulkRequest() # IdentityApiUserV1AddSectionBulkRequest |  (optional)

    try:
        # Adds Sections to a user in bulk.
        api_response = api_instance.add_user_section_bulk(tenant_id, user_id, identity_api_user_v1_add_section_bulk_request=identity_api_user_v1_add_section_bulk_request)
        print("The response of UsersSectionsApi->add_user_section_bulk:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersSectionsApi->add_user_section_bulk: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **user_id** | **str**|  | 
 **identity_api_user_v1_add_section_bulk_request** | [**IdentityApiUserV1AddSectionBulkRequest**](IdentityApiUserV1AddSectionBulkRequest.md)|  | [optional] 

### Return type

[**IdentityApiUserV1SectionAddedBulkResponse**](IdentityApiUserV1SectionAddedBulkResponse.md)

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

# **get_user_sections**
> IdentityApiUserV1GetSectionsResponse get_user_sections(tenant_id, user_id)

Gets the Sections of a user.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v1_get_sections_response import IdentityApiUserV1GetSectionsResponse
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
    api_instance = edgraph_platform_client.UsersSectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    user_id = 'user_id_example' # str | 

    try:
        # Gets the Sections of a user.
        api_response = api_instance.get_user_sections(tenant_id, user_id)
        print("The response of UsersSectionsApi->get_user_sections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersSectionsApi->get_user_sections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **user_id** | **str**|  | 

### Return type

[**IdentityApiUserV1GetSectionsResponse**](IdentityApiUserV1GetSectionsResponse.md)

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

# **remove_user_section**
> IdentityApiUserV1SectionRemovedResponse remove_user_section(tenant_id, user_id, user_section_id)

Removes a Section from a user.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v1_section_removed_response import IdentityApiUserV1SectionRemovedResponse
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
    api_instance = edgraph_platform_client.UsersSectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    user_id = 'user_id_example' # str | 
    user_section_id = 'user_section_id_example' # str | 

    try:
        # Removes a Section from a user.
        api_response = api_instance.remove_user_section(tenant_id, user_id, user_section_id)
        print("The response of UsersSectionsApi->remove_user_section:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersSectionsApi->remove_user_section: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **user_id** | **str**|  | 
 **user_section_id** | **str**|  | 

### Return type

[**IdentityApiUserV1SectionRemovedResponse**](IdentityApiUserV1SectionRemovedResponse.md)

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

# **remove_user_section_bulk**
> IdentityApiUserV1SectionRemovedBulkResponse remove_user_section_bulk(tenant_id, user_id, identity_api_user_v1_remove_section_bulk_request=identity_api_user_v1_remove_section_bulk_request)

Removes Sections from a user in bulk.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v1_remove_section_bulk_request import IdentityApiUserV1RemoveSectionBulkRequest
from edgraph_platform_client.models.identity_api_user_v1_section_removed_bulk_response import IdentityApiUserV1SectionRemovedBulkResponse
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
    api_instance = edgraph_platform_client.UsersSectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    user_id = 'user_id_example' # str | 
    identity_api_user_v1_remove_section_bulk_request = edgraph_platform_client.IdentityApiUserV1RemoveSectionBulkRequest() # IdentityApiUserV1RemoveSectionBulkRequest |  (optional)

    try:
        # Removes Sections from a user in bulk.
        api_response = api_instance.remove_user_section_bulk(tenant_id, user_id, identity_api_user_v1_remove_section_bulk_request=identity_api_user_v1_remove_section_bulk_request)
        print("The response of UsersSectionsApi->remove_user_section_bulk:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersSectionsApi->remove_user_section_bulk: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **user_id** | **str**|  | 
 **identity_api_user_v1_remove_section_bulk_request** | [**IdentityApiUserV1RemoveSectionBulkRequest**](IdentityApiUserV1RemoveSectionBulkRequest.md)|  | [optional] 

### Return type

[**IdentityApiUserV1SectionRemovedBulkResponse**](IdentityApiUserV1SectionRemovedBulkResponse.md)

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

# **update_user_section**
> IdentityApiUserV1SectionUpdatedResponse update_user_section(tenant_id, user_id, user_section_id, identity_api_user_v1_update_section_request=identity_api_user_v1_update_section_request)

Updates the Section of a user.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v1_section_updated_response import IdentityApiUserV1SectionUpdatedResponse
from edgraph_platform_client.models.identity_api_user_v1_update_section_request import IdentityApiUserV1UpdateSectionRequest
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
    api_instance = edgraph_platform_client.UsersSectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    user_id = 'user_id_example' # str | 
    user_section_id = 'user_section_id_example' # str | 
    identity_api_user_v1_update_section_request = edgraph_platform_client.IdentityApiUserV1UpdateSectionRequest() # IdentityApiUserV1UpdateSectionRequest |  (optional)

    try:
        # Updates the Section of a user.
        api_response = api_instance.update_user_section(tenant_id, user_id, user_section_id, identity_api_user_v1_update_section_request=identity_api_user_v1_update_section_request)
        print("The response of UsersSectionsApi->update_user_section:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersSectionsApi->update_user_section: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **user_id** | **str**|  | 
 **user_section_id** | **str**|  | 
 **identity_api_user_v1_update_section_request** | [**IdentityApiUserV1UpdateSectionRequest**](IdentityApiUserV1UpdateSectionRequest.md)|  | [optional] 

### Return type

[**IdentityApiUserV1SectionUpdatedResponse**](IdentityApiUserV1SectionUpdatedResponse.md)

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

# **update_user_section_bulk**
> IdentityApiUserV1SectionUpdatedBulkResponse update_user_section_bulk(tenant_id, user_id, identity_api_user_v1_update_section_bulk_request=identity_api_user_v1_update_section_bulk_request)

Updates the Section of a user in bulk.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v1_section_updated_bulk_response import IdentityApiUserV1SectionUpdatedBulkResponse
from edgraph_platform_client.models.identity_api_user_v1_update_section_bulk_request import IdentityApiUserV1UpdateSectionBulkRequest
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
    api_instance = edgraph_platform_client.UsersSectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    user_id = 'user_id_example' # str | 
    identity_api_user_v1_update_section_bulk_request = edgraph_platform_client.IdentityApiUserV1UpdateSectionBulkRequest() # IdentityApiUserV1UpdateSectionBulkRequest |  (optional)

    try:
        # Updates the Section of a user in bulk.
        api_response = api_instance.update_user_section_bulk(tenant_id, user_id, identity_api_user_v1_update_section_bulk_request=identity_api_user_v1_update_section_bulk_request)
        print("The response of UsersSectionsApi->update_user_section_bulk:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersSectionsApi->update_user_section_bulk: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **user_id** | **str**|  | 
 **identity_api_user_v1_update_section_bulk_request** | [**IdentityApiUserV1UpdateSectionBulkRequest**](IdentityApiUserV1UpdateSectionBulkRequest.md)|  | [optional] 

### Return type

[**IdentityApiUserV1SectionUpdatedBulkResponse**](IdentityApiUserV1SectionUpdatedBulkResponse.md)

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

