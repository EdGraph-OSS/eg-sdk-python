# edgraph_platform_client.EnrollmentAdminStudentsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_enrollment_student**](EnrollmentAdminStudentsApi.md#get_enrollment_student) | **GET** /tenants/{tenantId}/enrollmentadmin/students/{studentId} | Gets an Enrollment Student.
[**get_enrollment_students**](EnrollmentAdminStudentsApi.md#get_enrollment_students) | **GET** /tenants/{tenantId}/enrollmentadmin/students | Searches Enrollment Students.


# **get_enrollment_student**
> EnrollmentApiEnrollmentStudentsV1StudentResponse get_enrollment_student(tenant_id, student_id)

Gets an Enrollment Student.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.enrollment_api_enrollment_students_v1_student_response import EnrollmentApiEnrollmentStudentsV1StudentResponse
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
    api_instance = edgraph_platform_client.EnrollmentAdminStudentsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    student_id = 'student_id_example' # str | 

    try:
        # Gets an Enrollment Student.
        api_response = await api_instance.get_enrollment_student(tenant_id, student_id)
        print("The response of EnrollmentAdminStudentsApi->get_enrollment_student:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminStudentsApi->get_enrollment_student: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **student_id** | **str**|  | 

### Return type

[**EnrollmentApiEnrollmentStudentsV1StudentResponse**](EnrollmentApiEnrollmentStudentsV1StudentResponse.md)

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

# **get_enrollment_students**
> EnrollmentApiEnrollmentStudentsV1StudentsSearchResponse get_enrollment_students(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)

Searches Enrollment Students.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.enrollment_api_enrollment_students_v1_students_search_response import EnrollmentApiEnrollmentStudentsV1StudentsSearchResponse
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
    api_instance = edgraph_platform_client.EnrollmentAdminStudentsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_index = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    filter = 'filter_example' # str |  (optional)
    order_by = 'order_by_example' # str |  (optional)

    try:
        # Searches Enrollment Students.
        api_response = await api_instance.get_enrollment_students(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)
        print("The response of EnrollmentAdminStudentsApi->get_enrollment_students:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminStudentsApi->get_enrollment_students: %s\n" % e)
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

[**EnrollmentApiEnrollmentStudentsV1StudentsSearchResponse**](EnrollmentApiEnrollmentStudentsV1StudentsSearchResponse.md)

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

