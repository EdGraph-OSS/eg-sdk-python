# edgraph_platform_client.EnrollmentAdminResponsesApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_enrollment_application_response**](EnrollmentAdminResponsesApi.md#get_enrollment_application_response) | **GET** /tenants/{tenantId}/enrollmentadmin/responses/{responseId} | Gets an Enrollment Application Response.
[**get_enrollment_application_responses**](EnrollmentAdminResponsesApi.md#get_enrollment_application_responses) | **GET** /tenants/{tenantId}/enrollmentadmin/responses | Searches Enrollment Application Responses.


# **get_enrollment_application_response**
> EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseResponse get_enrollment_application_response(tenant_id, response_id)

Gets an Enrollment Application Response.

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
    api_instance = edgraph_platform_client.EnrollmentAdminResponsesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    response_id = 'response_id_example' # str | 

    try:
        # Gets an Enrollment Application Response.
        api_response = await api_instance.get_enrollment_application_response(tenant_id, response_id)
        print("The response of EnrollmentAdminResponsesApi->get_enrollment_application_response:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminResponsesApi->get_enrollment_application_response: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **response_id** | **str**|  | 

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

# **get_enrollment_application_responses**
> EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponsesSearchResponse get_enrollment_application_responses(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)

Searches Enrollment Application Responses.

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
    api_instance = edgraph_platform_client.EnrollmentAdminResponsesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_index = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    filter = 'filter_example' # str |  (optional)
    order_by = 'order_by_example' # str |  (optional)

    try:
        # Searches Enrollment Application Responses.
        api_response = await api_instance.get_enrollment_application_responses(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)
        print("The response of EnrollmentAdminResponsesApi->get_enrollment_application_responses:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminResponsesApi->get_enrollment_application_responses: %s\n" % e)
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

