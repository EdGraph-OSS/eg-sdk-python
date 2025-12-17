# edgraph_platform_client.InstancesReportsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**generate_reports_async**](InstancesReportsApi.md#generate_reports_async) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/reports/generate | Queues a job to generate the report views in the ODS Database.
[**get_reports_status_async**](InstancesReportsApi.md#get_reports_status_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/reports/status | Retrieves the status of the report views in Instance.
[**get_schools_by_type_report_async**](InstancesReportsApi.md#get_schools_by_type_report_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/reports/schoolsbytype/{localEducationAgencyId} | Retrieves a \&quot;Schools By Type\&quot; report.
[**get_student_economic_situation_report_async**](InstancesReportsApi.md#get_student_economic_situation_report_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/reports/studentseconomicsituation/{localEducationAgencyId} | Retrieves a \&quot;Students Economic Situation\&quot; report.
[**get_student_enrollment_by_ethnicity_report**](InstancesReportsApi.md#get_student_enrollment_by_ethnicity_report) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/reports/studentenrollment/ethnicity/{localEducationAgencyId} | Retrieves a \&quot;Student Enrollment By Ethnicity\&quot; report.
[**get_student_enrollment_by_gender_report_async**](InstancesReportsApi.md#get_student_enrollment_by_gender_report_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/reports/studentenrollment/gender/{localEducationAgencyId} | Retrieves a \&quot;Student Enrollment By Gender\&quot; report.
[**get_student_enrollment_by_race_report_async**](InstancesReportsApi.md#get_student_enrollment_by_race_report_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/reports/studentenrollment/race/{localEducationAgencyId} | Retrieves a \&quot;Student Enrollment By Race\&quot; report.
[**get_students_by_program_report_async**](InstancesReportsApi.md#get_students_by_program_report_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/reports/studentsbyprogram/{localEducationAgencyId} | Retrieves a \&quot;Students By Program\&quot; report.
[**get_total_enrollments_report_async**](InstancesReportsApi.md#get_total_enrollments_report_async) | **GET** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/reports/totalenrollments/{localEducationAgencyId} | Retrieves a \&quot;Total Enrollments\&quot; report.


# **generate_reports_async**
> EdfiAdminApiEdfiAdminV1GenerateReportsResponse generate_reports_async(tenant_id, instance_id)

Queues a job to generate the report views in the ODS Database.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_generate_reports_response import EdfiAdminApiEdfiAdminV1GenerateReportsResponse
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
    api_instance = edgraph_platform_client.InstancesReportsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 

    try:
        # Queues a job to generate the report views in the ODS Database.
        api_response = api_instance.generate_reports_async(tenant_id, instance_id)
        print("The response of InstancesReportsApi->generate_reports_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesReportsApi->generate_reports_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1GenerateReportsResponse**](EdfiAdminApiEdfiAdminV1GenerateReportsResponse.md)

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

# **get_reports_status_async**
> EdfiAdminApiEdfiAdminV1ReportsStatusResponse get_reports_status_async(tenant_id, instance_id)

Retrieves the status of the report views in Instance.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_reports_status_response import EdfiAdminApiEdfiAdminV1ReportsStatusResponse
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
    api_instance = edgraph_platform_client.InstancesReportsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 

    try:
        # Retrieves the status of the report views in Instance.
        api_response = api_instance.get_reports_status_async(tenant_id, instance_id)
        print("The response of InstancesReportsApi->get_reports_status_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesReportsApi->get_reports_status_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1ReportsStatusResponse**](EdfiAdminApiEdfiAdminV1ReportsStatusResponse.md)

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

# **get_schools_by_type_report_async**
> EdfiAdminApiEdfiAdminV1SchoolsByTypeReportResponse get_schools_by_type_report_async(tenant_id, instance_id, local_education_agency_id)

Retrieves a \"Schools By Type\" report.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_schools_by_type_report_response import EdfiAdminApiEdfiAdminV1SchoolsByTypeReportResponse
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
    api_instance = edgraph_platform_client.InstancesReportsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    local_education_agency_id = 56 # int | 

    try:
        # Retrieves a \"Schools By Type\" report.
        api_response = api_instance.get_schools_by_type_report_async(tenant_id, instance_id, local_education_agency_id)
        print("The response of InstancesReportsApi->get_schools_by_type_report_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesReportsApi->get_schools_by_type_report_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **local_education_agency_id** | **int**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1SchoolsByTypeReportResponse**](EdfiAdminApiEdfiAdminV1SchoolsByTypeReportResponse.md)

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

# **get_student_economic_situation_report_async**
> EdfiAdminApiEdfiAdminV1StudentEconomicSituationReportResponse get_student_economic_situation_report_async(tenant_id, instance_id, local_education_agency_id)

Retrieves a \"Students Economic Situation\" report.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_student_economic_situation_report_response import EdfiAdminApiEdfiAdminV1StudentEconomicSituationReportResponse
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
    api_instance = edgraph_platform_client.InstancesReportsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    local_education_agency_id = 56 # int | 

    try:
        # Retrieves a \"Students Economic Situation\" report.
        api_response = api_instance.get_student_economic_situation_report_async(tenant_id, instance_id, local_education_agency_id)
        print("The response of InstancesReportsApi->get_student_economic_situation_report_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesReportsApi->get_student_economic_situation_report_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **local_education_agency_id** | **int**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1StudentEconomicSituationReportResponse**](EdfiAdminApiEdfiAdminV1StudentEconomicSituationReportResponse.md)

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

# **get_student_enrollment_by_ethnicity_report**
> EdfiAdminApiEdfiAdminV1StudentEnrollmentByEthnicityReportResponse get_student_enrollment_by_ethnicity_report(tenant_id, instance_id, local_education_agency_id)

Retrieves a \"Student Enrollment By Ethnicity\" report.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_student_enrollment_by_ethnicity_report_response import EdfiAdminApiEdfiAdminV1StudentEnrollmentByEthnicityReportResponse
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
    api_instance = edgraph_platform_client.InstancesReportsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    local_education_agency_id = 56 # int | 

    try:
        # Retrieves a \"Student Enrollment By Ethnicity\" report.
        api_response = api_instance.get_student_enrollment_by_ethnicity_report(tenant_id, instance_id, local_education_agency_id)
        print("The response of InstancesReportsApi->get_student_enrollment_by_ethnicity_report:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesReportsApi->get_student_enrollment_by_ethnicity_report: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **local_education_agency_id** | **int**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1StudentEnrollmentByEthnicityReportResponse**](EdfiAdminApiEdfiAdminV1StudentEnrollmentByEthnicityReportResponse.md)

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

# **get_student_enrollment_by_gender_report_async**
> EdfiAdminApiEdfiAdminV1StudentEnrollmentByGenderReportResponse get_student_enrollment_by_gender_report_async(tenant_id, instance_id, local_education_agency_id)

Retrieves a \"Student Enrollment By Gender\" report.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_student_enrollment_by_gender_report_response import EdfiAdminApiEdfiAdminV1StudentEnrollmentByGenderReportResponse
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
    api_instance = edgraph_platform_client.InstancesReportsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    local_education_agency_id = 56 # int | 

    try:
        # Retrieves a \"Student Enrollment By Gender\" report.
        api_response = api_instance.get_student_enrollment_by_gender_report_async(tenant_id, instance_id, local_education_agency_id)
        print("The response of InstancesReportsApi->get_student_enrollment_by_gender_report_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesReportsApi->get_student_enrollment_by_gender_report_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **local_education_agency_id** | **int**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1StudentEnrollmentByGenderReportResponse**](EdfiAdminApiEdfiAdminV1StudentEnrollmentByGenderReportResponse.md)

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

# **get_student_enrollment_by_race_report_async**
> EdfiAdminApiEdfiAdminV1StudentEnrollmentByRaceReportResponse get_student_enrollment_by_race_report_async(tenant_id, instance_id, local_education_agency_id)

Retrieves a \"Student Enrollment By Race\" report.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_student_enrollment_by_race_report_response import EdfiAdminApiEdfiAdminV1StudentEnrollmentByRaceReportResponse
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
    api_instance = edgraph_platform_client.InstancesReportsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    local_education_agency_id = 56 # int | 

    try:
        # Retrieves a \"Student Enrollment By Race\" report.
        api_response = api_instance.get_student_enrollment_by_race_report_async(tenant_id, instance_id, local_education_agency_id)
        print("The response of InstancesReportsApi->get_student_enrollment_by_race_report_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesReportsApi->get_student_enrollment_by_race_report_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **local_education_agency_id** | **int**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1StudentEnrollmentByRaceReportResponse**](EdfiAdminApiEdfiAdminV1StudentEnrollmentByRaceReportResponse.md)

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

# **get_students_by_program_report_async**
> EdfiAdminApiEdfiAdminV1StudentsByProgramReportResponse get_students_by_program_report_async(tenant_id, instance_id, local_education_agency_id)

Retrieves a \"Students By Program\" report.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_students_by_program_report_response import EdfiAdminApiEdfiAdminV1StudentsByProgramReportResponse
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
    api_instance = edgraph_platform_client.InstancesReportsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    local_education_agency_id = 56 # int | 

    try:
        # Retrieves a \"Students By Program\" report.
        api_response = api_instance.get_students_by_program_report_async(tenant_id, instance_id, local_education_agency_id)
        print("The response of InstancesReportsApi->get_students_by_program_report_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesReportsApi->get_students_by_program_report_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **local_education_agency_id** | **int**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1StudentsByProgramReportResponse**](EdfiAdminApiEdfiAdminV1StudentsByProgramReportResponse.md)

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

# **get_total_enrollments_report_async**
> EdfiAdminApiEdfiAdminV1TotalEnrollmentsReportResponse get_total_enrollments_report_async(tenant_id, instance_id, local_education_agency_id)

Retrieves a \"Total Enrollments\" report.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_total_enrollments_report_response import EdfiAdminApiEdfiAdminV1TotalEnrollmentsReportResponse
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
    api_instance = edgraph_platform_client.InstancesReportsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    local_education_agency_id = 56 # int | 

    try:
        # Retrieves a \"Total Enrollments\" report.
        api_response = api_instance.get_total_enrollments_report_async(tenant_id, instance_id, local_education_agency_id)
        print("The response of InstancesReportsApi->get_total_enrollments_report_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstancesReportsApi->get_total_enrollments_report_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **local_education_agency_id** | **int**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1TotalEnrollmentsReportResponse**](EdfiAdminApiEdfiAdminV1TotalEnrollmentsReportResponse.md)

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

