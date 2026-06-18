# edgraph_platform_client.StaffClassificationsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_staff_classification**](StaffClassificationsApi.md#create_staff_classification) | **POST** /tenants/{tenantId}/staffclassifications | Creates a StaffClassification.
[**delete_staff_classification**](StaffClassificationsApi.md#delete_staff_classification) | **DELETE** /tenants/{tenantId}/staffclassifications/{staffClassificationId} | Deletes a StaffClassification.
[**get_staff_classification_by_id**](StaffClassificationsApi.md#get_staff_classification_by_id) | **GET** /tenants/{tenantId}/staffclassifications/{staffClassificationId} | Retrieves a StaffClassification by ID.
[**get_staff_classifications**](StaffClassificationsApi.md#get_staff_classifications) | **GET** /tenants/{tenantId}/staffclassifications | Retrieves a list of StaffClassifications.
[**get_staff_classifications_namespaces**](StaffClassificationsApi.md#get_staff_classifications_namespaces) | **GET** /tenants/{tenantId}/staffclassifications/namespaces | Retrieves a list of unique Staff Classification Namespaces.
[**update_staff_classification**](StaffClassificationsApi.md#update_staff_classification) | **PUT** /tenants/{tenantId}/staffclassifications/{staffClassificationId} | Updates a StaffClassification.


# **create_staff_classification**
> IdentityApiStaffClassificationV1StaffClassificationCreatedResponse create_staff_classification(tenant_id, identity_api_staff_classification_v1_create_staff_classification_request=identity_api_staff_classification_v1_create_staff_classification_request)

Creates a StaffClassification.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_staff_classification_v1_create_staff_classification_request import IdentityApiStaffClassificationV1CreateStaffClassificationRequest
from edgraph_platform_client.models.identity_api_staff_classification_v1_staff_classification_created_response import IdentityApiStaffClassificationV1StaffClassificationCreatedResponse
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
    api_instance = edgraph_platform_client.StaffClassificationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    identity_api_staff_classification_v1_create_staff_classification_request = edgraph_platform_client.IdentityApiStaffClassificationV1CreateStaffClassificationRequest() # IdentityApiStaffClassificationV1CreateStaffClassificationRequest |  (optional)

    try:
        # Creates a StaffClassification.
        api_response = await api_instance.create_staff_classification(tenant_id, identity_api_staff_classification_v1_create_staff_classification_request=identity_api_staff_classification_v1_create_staff_classification_request)
        print("The response of StaffClassificationsApi->create_staff_classification:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffClassificationsApi->create_staff_classification: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **identity_api_staff_classification_v1_create_staff_classification_request** | [**IdentityApiStaffClassificationV1CreateStaffClassificationRequest**](IdentityApiStaffClassificationV1CreateStaffClassificationRequest.md)|  | [optional] 

### Return type

[**IdentityApiStaffClassificationV1StaffClassificationCreatedResponse**](IdentityApiStaffClassificationV1StaffClassificationCreatedResponse.md)

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

# **delete_staff_classification**
> IdentityApiStaffClassificationV1StaffClassificationDeletedResponse delete_staff_classification(tenant_id, staff_classification_id)

Deletes a StaffClassification.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_staff_classification_v1_staff_classification_deleted_response import IdentityApiStaffClassificationV1StaffClassificationDeletedResponse
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
    api_instance = edgraph_platform_client.StaffClassificationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    staff_classification_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Deletes a StaffClassification.
        api_response = await api_instance.delete_staff_classification(tenant_id, staff_classification_id)
        print("The response of StaffClassificationsApi->delete_staff_classification:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffClassificationsApi->delete_staff_classification: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **staff_classification_id** | **UUID**|  | 

### Return type

[**IdentityApiStaffClassificationV1StaffClassificationDeletedResponse**](IdentityApiStaffClassificationV1StaffClassificationDeletedResponse.md)

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

# **get_staff_classification_by_id**
> IdentityApiStaffClassificationV1StaffClassificationResponse get_staff_classification_by_id(tenant_id, staff_classification_id)

Retrieves a StaffClassification by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_staff_classification_v1_staff_classification_response import IdentityApiStaffClassificationV1StaffClassificationResponse
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
    api_instance = edgraph_platform_client.StaffClassificationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    staff_classification_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Retrieves a StaffClassification by ID.
        api_response = await api_instance.get_staff_classification_by_id(tenant_id, staff_classification_id)
        print("The response of StaffClassificationsApi->get_staff_classification_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffClassificationsApi->get_staff_classification_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **staff_classification_id** | **UUID**|  | 

### Return type

[**IdentityApiStaffClassificationV1StaffClassificationResponse**](IdentityApiStaffClassificationV1StaffClassificationResponse.md)

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

# **get_staff_classifications**
> IdentityApiStaffClassificationV1GetStaffClassificationsResponse get_staff_classifications(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)

Retrieves a list of StaffClassifications.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_staff_classification_v1_get_staff_classifications_response import IdentityApiStaffClassificationV1GetStaffClassificationsResponse
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
    api_instance = edgraph_platform_client.StaffClassificationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of StaffClassifications.
        api_response = await api_instance.get_staff_classifications(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)
        print("The response of StaffClassificationsApi->get_staff_classifications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffClassificationsApi->get_staff_classifications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**IdentityApiStaffClassificationV1GetStaffClassificationsResponse**](IdentityApiStaffClassificationV1GetStaffClassificationsResponse.md)

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

# **get_staff_classifications_namespaces**
> IdentityApiStaffClassificationV1GetStaffClassificationsNamespacesResponse get_staff_classifications_namespaces(tenant_id, page_index=page_index, page_size=page_size, filter=filter)

Retrieves a list of unique Staff Classification Namespaces.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_staff_classification_v1_get_staff_classifications_namespaces_response import IdentityApiStaffClassificationV1GetStaffClassificationsNamespacesResponse
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
    api_instance = edgraph_platform_client.StaffClassificationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of unique Staff Classification Namespaces.
        api_response = await api_instance.get_staff_classifications_namespaces(tenant_id, page_index=page_index, page_size=page_size, filter=filter)
        print("The response of StaffClassificationsApi->get_staff_classifications_namespaces:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffClassificationsApi->get_staff_classifications_namespaces: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**IdentityApiStaffClassificationV1GetStaffClassificationsNamespacesResponse**](IdentityApiStaffClassificationV1GetStaffClassificationsNamespacesResponse.md)

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

# **update_staff_classification**
> IdentityApiStaffClassificationV1StaffClassificationUpdatedResponse update_staff_classification(tenant_id, staff_classification_id, identity_api_staff_classification_v1_update_staff_classification_request=identity_api_staff_classification_v1_update_staff_classification_request)

Updates a StaffClassification.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_staff_classification_v1_staff_classification_updated_response import IdentityApiStaffClassificationV1StaffClassificationUpdatedResponse
from edgraph_platform_client.models.identity_api_staff_classification_v1_update_staff_classification_request import IdentityApiStaffClassificationV1UpdateStaffClassificationRequest
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
    api_instance = edgraph_platform_client.StaffClassificationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    staff_classification_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    identity_api_staff_classification_v1_update_staff_classification_request = edgraph_platform_client.IdentityApiStaffClassificationV1UpdateStaffClassificationRequest() # IdentityApiStaffClassificationV1UpdateStaffClassificationRequest |  (optional)

    try:
        # Updates a StaffClassification.
        api_response = await api_instance.update_staff_classification(tenant_id, staff_classification_id, identity_api_staff_classification_v1_update_staff_classification_request=identity_api_staff_classification_v1_update_staff_classification_request)
        print("The response of StaffClassificationsApi->update_staff_classification:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffClassificationsApi->update_staff_classification: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **staff_classification_id** | **UUID**|  | 
 **identity_api_staff_classification_v1_update_staff_classification_request** | [**IdentityApiStaffClassificationV1UpdateStaffClassificationRequest**](IdentityApiStaffClassificationV1UpdateStaffClassificationRequest.md)|  | [optional] 

### Return type

[**IdentityApiStaffClassificationV1StaffClassificationUpdatedResponse**](IdentityApiStaffClassificationV1StaffClassificationUpdatedResponse.md)

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

