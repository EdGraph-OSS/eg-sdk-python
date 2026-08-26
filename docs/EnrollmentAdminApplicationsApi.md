# edgraph_platform_client.EnrollmentAdminApplicationsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_enrollment_application**](EnrollmentAdminApplicationsApi.md#get_enrollment_application) | **GET** /tenants/{tenantId}/enrollmentadmin/applications/{applicationId} | Gets an Enrollment Application.
[**get_enrollment_applications**](EnrollmentAdminApplicationsApi.md#get_enrollment_applications) | **GET** /tenants/{tenantId}/enrollmentadmin/applications | Searches Enrollment Applications.


# **get_enrollment_application**
> EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseResponse get_enrollment_application(tenant_id, application_id)

Gets an Enrollment Application.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.enrollment_api_enrollment_application_responses_v1_application_response_response import EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseResponse
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
    api_instance = edgraph_platform_client.EnrollmentAdminApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    application_id = 'application_id_example' # str | 

    try:
        # Gets an Enrollment Application.
        api_response = await api_instance.get_enrollment_application(tenant_id, application_id)
        print("The response of EnrollmentAdminApplicationsApi->get_enrollment_application:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminApplicationsApi->get_enrollment_application: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **application_id** | **str**|  | 

### Return type

[**EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseResponse**](EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_enrollment_applications**
> EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponsesSearchResponse get_enrollment_applications(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)

Searches Enrollment Applications.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.enrollment_api_enrollment_application_responses_v1_application_responses_search_response import EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponsesSearchResponse
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
    api_instance = edgraph_platform_client.EnrollmentAdminApplicationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_index = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    filter = 'filter_example' # str |  (optional)
    order_by = 'order_by_example' # str |  (optional)

    try:
        # Searches Enrollment Applications.
        api_response = await api_instance.get_enrollment_applications(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)
        print("The response of EnrollmentAdminApplicationsApi->get_enrollment_applications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminApplicationsApi->get_enrollment_applications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_index** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **filter** | **str**|  | [optional] 
 **order_by** | **str**|  | [optional] 

### Return type

[**EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponsesSearchResponse**](EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponsesSearchResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The requested resource was successfully retrieved. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

