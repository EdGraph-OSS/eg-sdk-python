# edgraph_platform_client.RegistrationsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_onboarding_applications_async**](RegistrationsApi.md#get_onboarding_applications_async) | **GET** /public/applications | Gets a list of applications available for registration/onboarding
[**get_registration_approval_status_async**](RegistrationsApi.md#get_registration_approval_status_async) | **GET** /registrations/{registrationId} | Gets the approval status of a registration
[**submit_tenant_registration_async**](RegistrationsApi.md#submit_tenant_registration_async) | **POST** /registrations | Submits a tenant&#39;s registration request


# **get_onboarding_applications_async**
> ApplicationApiApplicationV1PaginatedItemsResponse get_onboarding_applications_async(page_size=page_size, page_index=page_index, order_by=order_by)

Gets a list of applications available for registration/onboarding

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.application_api_application_v1_paginated_items_response import ApplicationApiApplicationV1PaginatedItemsResponse
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
    api_instance = edgraph_platform_client.RegistrationsApi(api_client)
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')

    try:
        # Gets a list of applications available for registration/onboarding
        api_response = await api_instance.get_onboarding_applications_async(page_size=page_size, page_index=page_index, order_by=order_by)
        print("The response of RegistrationsApi->get_onboarding_applications_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RegistrationsApi->get_onboarding_applications_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**ApplicationApiApplicationV1PaginatedItemsResponse**](ApplicationApiApplicationV1PaginatedItemsResponse.md)

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

# **get_registration_approval_status_async**
> RegistrationApiRegistrationV2ApprovalStatus get_registration_approval_status_async(registration_id)

Gets the approval status of a registration

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.registration_api_registration_v2_approval_status import RegistrationApiRegistrationV2ApprovalStatus
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
    api_instance = edgraph_platform_client.RegistrationsApi(api_client)
    registration_id = 'registration_id_example' # str | 

    try:
        # Gets the approval status of a registration
        api_response = await api_instance.get_registration_approval_status_async(registration_id)
        print("The response of RegistrationsApi->get_registration_approval_status_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RegistrationsApi->get_registration_approval_status_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registration_id** | **str**|  | 

### Return type

[**RegistrationApiRegistrationV2ApprovalStatus**](RegistrationApiRegistrationV2ApprovalStatus.md)

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

# **submit_tenant_registration_async**
> str submit_tenant_registration_async(registration_api_registration_v2_submit_tenant_registration_request=registration_api_registration_v2_submit_tenant_registration_request)

Submits a tenant's registration request

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.registration_api_registration_v2_submit_tenant_registration_request import RegistrationApiRegistrationV2SubmitTenantRegistrationRequest
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
    api_instance = edgraph_platform_client.RegistrationsApi(api_client)
    registration_api_registration_v2_submit_tenant_registration_request = edgraph_platform_client.RegistrationApiRegistrationV2SubmitTenantRegistrationRequest() # RegistrationApiRegistrationV2SubmitTenantRegistrationRequest |  (optional)

    try:
        # Submits a tenant's registration request
        api_response = await api_instance.submit_tenant_registration_async(registration_api_registration_v2_submit_tenant_registration_request=registration_api_registration_v2_submit_tenant_registration_request)
        print("The response of RegistrationsApi->submit_tenant_registration_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RegistrationsApi->submit_tenant_registration_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registration_api_registration_v2_submit_tenant_registration_request** | [**RegistrationApiRegistrationV2SubmitTenantRegistrationRequest**](RegistrationApiRegistrationV2SubmitTenantRegistrationRequest.md)|  | [optional] 

### Return type

**str**

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

