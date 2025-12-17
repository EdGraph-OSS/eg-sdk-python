# edgraph_platform_client.EnvironmentsReportingPeriodsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancel_state_reporting_period_run**](EnvironmentsReportingPeriodsApi.md#cancel_state_reporting_period_run) | **DELETE** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/run | Cancel the Validation Run of a Reporting Period.
[**close_state_reporting_period**](EnvironmentsReportingPeriodsApi.md#close_state_reporting_period) | **PUT** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/close | Closes a Reporting Period.
[**create_state_reporting_period**](EnvironmentsReportingPeriodsApi.md#create_state_reporting_period) | **POST** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods | Creates a new Reporting Period.
[**delete_state_reporting_period**](EnvironmentsReportingPeriodsApi.md#delete_state_reporting_period) | **DELETE** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId} | Deletes a Reporting Period.
[**get_state_reporting_period**](EnvironmentsReportingPeriodsApi.md#get_state_reporting_period) | **GET** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId} | Retrieves a Reporting Period by ID.
[**get_state_reporting_period_certification_status**](EnvironmentsReportingPeriodsApi.md#get_state_reporting_period_certification_status) | **GET** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/certificationstatus | Retrieves the Certification Status of Reporting Period.
[**get_state_reporting_period_validation_summary**](EnvironmentsReportingPeriodsApi.md#get_state_reporting_period_validation_summary) | **GET** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/validationsummary | Retrieves the Validation Summary of Reporting Period.
[**get_state_reporting_period_validation_summary_by_category**](EnvironmentsReportingPeriodsApi.md#get_state_reporting_period_validation_summary_by_category) | **GET** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/validationsummary/categories/{categoryId} | Retrieves the Validation Summary of Reporting Period by Category.
[**post_state_reporting_period**](EnvironmentsReportingPeriodsApi.md#post_state_reporting_period) | **POST** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/post | Posts a Reporting Period.
[**run_state_reporting_period**](EnvironmentsReportingPeriodsApi.md#run_state_reporting_period) | **POST** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/run | Run a Reporting Period.
[**search_state_reporting_periods**](EnvironmentsReportingPeriodsApi.md#search_state_reporting_periods) | **GET** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods | Retrieves a list of Reporting Periods.
[**set_state_reporting_period_current_step**](EnvironmentsReportingPeriodsApi.md#set_state_reporting_period_current_step) | **PUT** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/steps/current | Sets the current step of a Reporting Period.
[**set_state_reporting_period_step_status**](EnvironmentsReportingPeriodsApi.md#set_state_reporting_period_step_status) | **PUT** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/steps/{stepNumber} | Sets the status of a Reporting Period step.
[**toggle_state_reporting_period_selected**](EnvironmentsReportingPeriodsApi.md#toggle_state_reporting_period_selected) | **PUT** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/toggle | Toggles the Selected state of a Reporting Period.
[**update_state_reporting_period**](EnvironmentsReportingPeriodsApi.md#update_state_reporting_period) | **PUT** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId} | Updates a Reporting Period.
[**update_state_reporting_period_bulk**](EnvironmentsReportingPeriodsApi.md#update_state_reporting_period_bulk) | **PUT** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods | Updates Reporting Periods in bulk.


# **cancel_state_reporting_period_run**
> EdGraphServicesStateReportingV1ReportingPeriodValidationsCancelledResponse cancel_state_reporting_period_run(tenant_id, environment_id, reporting_period_id)

Cancel the Validation Run of a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_validations_cancelled_response import EdGraphServicesStateReportingV1ReportingPeriodValidationsCancelledResponse
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 

    try:
        # Cancel the Validation Run of a Reporting Period.
        api_response = api_instance.cancel_state_reporting_period_run(tenant_id, environment_id, reporting_period_id)
        print("The response of EnvironmentsReportingPeriodsApi->cancel_state_reporting_period_run:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsApi->cancel_state_reporting_period_run: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 

### Return type

[**EdGraphServicesStateReportingV1ReportingPeriodValidationsCancelledResponse**](EdGraphServicesStateReportingV1ReportingPeriodValidationsCancelledResponse.md)

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
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **close_state_reporting_period**
> EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse close_state_reporting_period(tenant_id, environment_id, reporting_period_id)

Closes a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_created_response import EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 

    try:
        # Closes a Reporting Period.
        api_response = api_instance.close_state_reporting_period(tenant_id, environment_id, reporting_period_id)
        print("The response of EnvironmentsReportingPeriodsApi->close_state_reporting_period:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsApi->close_state_reporting_period: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 

### Return type

[**EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse**](EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse.md)

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
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**201** | The resource was created. The location of the resource is available in the Location header of the response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_state_reporting_period**
> EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse create_state_reporting_period(tenant_id, environment_id, ed_graph_services_state_reporting_v1_create_reporting_period_request=ed_graph_services_state_reporting_v1_create_reporting_period_request)

Creates a new Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_create_reporting_period_request import EdGraphServicesStateReportingV1CreateReportingPeriodRequest
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_created_response import EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    ed_graph_services_state_reporting_v1_create_reporting_period_request = edgraph_platform_client.EdGraphServicesStateReportingV1CreateReportingPeriodRequest() # EdGraphServicesStateReportingV1CreateReportingPeriodRequest |  (optional)

    try:
        # Creates a new Reporting Period.
        api_response = api_instance.create_state_reporting_period(tenant_id, environment_id, ed_graph_services_state_reporting_v1_create_reporting_period_request=ed_graph_services_state_reporting_v1_create_reporting_period_request)
        print("The response of EnvironmentsReportingPeriodsApi->create_state_reporting_period:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsApi->create_state_reporting_period: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **ed_graph_services_state_reporting_v1_create_reporting_period_request** | [**EdGraphServicesStateReportingV1CreateReportingPeriodRequest**](EdGraphServicesStateReportingV1CreateReportingPeriodRequest.md)|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse**](EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse.md)

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
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**201** | The resource was created. The location of the resource is available in the Location header of the response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_state_reporting_period**
> EdGraphServicesStateReportingV1ReportingPeriodDeletedResponse delete_state_reporting_period(tenant_id, environment_id, reporting_period_id)

Deletes a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_deleted_response import EdGraphServicesStateReportingV1ReportingPeriodDeletedResponse
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 

    try:
        # Deletes a Reporting Period.
        api_response = api_instance.delete_state_reporting_period(tenant_id, environment_id, reporting_period_id)
        print("The response of EnvironmentsReportingPeriodsApi->delete_state_reporting_period:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsApi->delete_state_reporting_period: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 

### Return type

[**EdGraphServicesStateReportingV1ReportingPeriodDeletedResponse**](EdGraphServicesStateReportingV1ReportingPeriodDeletedResponse.md)

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
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_state_reporting_period**
> EdGraphServicesStateReportingV1ReportingPeriodProfileResponse get_state_reporting_period(tenant_id, environment_id, reporting_period_id)

Retrieves a Reporting Period by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_profile_response import EdGraphServicesStateReportingV1ReportingPeriodProfileResponse
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 

    try:
        # Retrieves a Reporting Period by ID.
        api_response = api_instance.get_state_reporting_period(tenant_id, environment_id, reporting_period_id)
        print("The response of EnvironmentsReportingPeriodsApi->get_state_reporting_period:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsApi->get_state_reporting_period: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 

### Return type

[**EdGraphServicesStateReportingV1ReportingPeriodProfileResponse**](EdGraphServicesStateReportingV1ReportingPeriodProfileResponse.md)

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

# **get_state_reporting_period_certification_status**
> EdGraphServicesStateReportingV1ReportingPeriodCertificationStatus get_state_reporting_period_certification_status(tenant_id, environment_id, reporting_period_id)

Retrieves the Certification Status of Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_certification_status import EdGraphServicesStateReportingV1ReportingPeriodCertificationStatus
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 

    try:
        # Retrieves the Certification Status of Reporting Period.
        api_response = api_instance.get_state_reporting_period_certification_status(tenant_id, environment_id, reporting_period_id)
        print("The response of EnvironmentsReportingPeriodsApi->get_state_reporting_period_certification_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsApi->get_state_reporting_period_certification_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 

### Return type

[**EdGraphServicesStateReportingV1ReportingPeriodCertificationStatus**](EdGraphServicesStateReportingV1ReportingPeriodCertificationStatus.md)

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

# **get_state_reporting_period_validation_summary**
> EdGraphServicesStateReportingV1ReportingPeriodValidationSummary get_state_reporting_period_validation_summary(tenant_id, environment_id, reporting_period_id)

Retrieves the Validation Summary of Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_validation_summary import EdGraphServicesStateReportingV1ReportingPeriodValidationSummary
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 

    try:
        # Retrieves the Validation Summary of Reporting Period.
        api_response = api_instance.get_state_reporting_period_validation_summary(tenant_id, environment_id, reporting_period_id)
        print("The response of EnvironmentsReportingPeriodsApi->get_state_reporting_period_validation_summary:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsApi->get_state_reporting_period_validation_summary: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 

### Return type

[**EdGraphServicesStateReportingV1ReportingPeriodValidationSummary**](EdGraphServicesStateReportingV1ReportingPeriodValidationSummary.md)

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

# **get_state_reporting_period_validation_summary_by_category**
> EdGraphServicesStateReportingV1ReportingPeriodValidationSummaryByCategoryId get_state_reporting_period_validation_summary_by_category(tenant_id, environment_id, reporting_period_id, category_id)

Retrieves the Validation Summary of Reporting Period by Category.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_validation_summary_by_category_id import EdGraphServicesStateReportingV1ReportingPeriodValidationSummaryByCategoryId
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    category_id = 'category_id_example' # str | 

    try:
        # Retrieves the Validation Summary of Reporting Period by Category.
        api_response = api_instance.get_state_reporting_period_validation_summary_by_category(tenant_id, environment_id, reporting_period_id, category_id)
        print("The response of EnvironmentsReportingPeriodsApi->get_state_reporting_period_validation_summary_by_category:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsApi->get_state_reporting_period_validation_summary_by_category: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **category_id** | **str**|  | 

### Return type

[**EdGraphServicesStateReportingV1ReportingPeriodValidationSummaryByCategoryId**](EdGraphServicesStateReportingV1ReportingPeriodValidationSummaryByCategoryId.md)

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

# **post_state_reporting_period**
> EdGraphServicesStateReportingV1ReportingPeriodPostedResponse post_state_reporting_period(tenant_id, environment_id, reporting_period_id, ed_graph_services_state_reporting_v1_post_reporting_period_request=ed_graph_services_state_reporting_v1_post_reporting_period_request)

Posts a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_post_reporting_period_request import EdGraphServicesStateReportingV1PostReportingPeriodRequest
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_posted_response import EdGraphServicesStateReportingV1ReportingPeriodPostedResponse
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    ed_graph_services_state_reporting_v1_post_reporting_period_request = edgraph_platform_client.EdGraphServicesStateReportingV1PostReportingPeriodRequest() # EdGraphServicesStateReportingV1PostReportingPeriodRequest |  (optional)

    try:
        # Posts a Reporting Period.
        api_response = api_instance.post_state_reporting_period(tenant_id, environment_id, reporting_period_id, ed_graph_services_state_reporting_v1_post_reporting_period_request=ed_graph_services_state_reporting_v1_post_reporting_period_request)
        print("The response of EnvironmentsReportingPeriodsApi->post_state_reporting_period:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsApi->post_state_reporting_period: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **ed_graph_services_state_reporting_v1_post_reporting_period_request** | [**EdGraphServicesStateReportingV1PostReportingPeriodRequest**](EdGraphServicesStateReportingV1PostReportingPeriodRequest.md)|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1ReportingPeriodPostedResponse**](EdGraphServicesStateReportingV1ReportingPeriodPostedResponse.md)

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
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**201** | The resource was created. The location of the resource is available in the Location header of the response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **run_state_reporting_period**
> EdGraphServicesStateReportingV1ReportingPeriodRunResponse run_state_reporting_period(tenant_id, environment_id, reporting_period_id, ed_graph_services_state_reporting_v1_run_reporting_period_request=ed_graph_services_state_reporting_v1_run_reporting_period_request)

Run a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_run_response import EdGraphServicesStateReportingV1ReportingPeriodRunResponse
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_run_reporting_period_request import EdGraphServicesStateReportingV1RunReportingPeriodRequest
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    ed_graph_services_state_reporting_v1_run_reporting_period_request = edgraph_platform_client.EdGraphServicesStateReportingV1RunReportingPeriodRequest() # EdGraphServicesStateReportingV1RunReportingPeriodRequest |  (optional)

    try:
        # Run a Reporting Period.
        api_response = api_instance.run_state_reporting_period(tenant_id, environment_id, reporting_period_id, ed_graph_services_state_reporting_v1_run_reporting_period_request=ed_graph_services_state_reporting_v1_run_reporting_period_request)
        print("The response of EnvironmentsReportingPeriodsApi->run_state_reporting_period:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsApi->run_state_reporting_period: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **ed_graph_services_state_reporting_v1_run_reporting_period_request** | [**EdGraphServicesStateReportingV1RunReportingPeriodRequest**](EdGraphServicesStateReportingV1RunReportingPeriodRequest.md)|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1ReportingPeriodRunResponse**](EdGraphServicesStateReportingV1ReportingPeriodRunResponse.md)

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
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**201** | The resource was created. The location of the resource is available in the Location header of the response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **search_state_reporting_periods**
> EdGraphServicesStateReportingV1PaginatedReportingPeriods search_state_reporting_periods(tenant_id, environment_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)

Retrieves a list of Reporting Periods.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_paginated_reporting_periods import EdGraphServicesStateReportingV1PaginatedReportingPeriods
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = 'order_by_example' # str |  (optional)
    filter = 'filter_example' # str |  (optional)

    try:
        # Retrieves a list of Reporting Periods.
        api_response = api_instance.search_state_reporting_periods(tenant_id, environment_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)
        print("The response of EnvironmentsReportingPeriodsApi->search_state_reporting_periods:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsApi->search_state_reporting_periods: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **order_by** | **str**|  | [optional] 
 **filter** | **str**|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1PaginatedReportingPeriods**](EdGraphServicesStateReportingV1PaginatedReportingPeriods.md)

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

# **set_state_reporting_period_current_step**
> EdGraphServicesStateReportingV1ReportingPeriodCurrentStepSetResponse set_state_reporting_period_current_step(tenant_id, environment_id, reporting_period_id, ed_graph_services_state_reporting_v1_set_reporting_period_current_step_request=ed_graph_services_state_reporting_v1_set_reporting_period_current_step_request)

Sets the current step of a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_current_step_set_response import EdGraphServicesStateReportingV1ReportingPeriodCurrentStepSetResponse
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_set_reporting_period_current_step_request import EdGraphServicesStateReportingV1SetReportingPeriodCurrentStepRequest
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    ed_graph_services_state_reporting_v1_set_reporting_period_current_step_request = edgraph_platform_client.EdGraphServicesStateReportingV1SetReportingPeriodCurrentStepRequest() # EdGraphServicesStateReportingV1SetReportingPeriodCurrentStepRequest |  (optional)

    try:
        # Sets the current step of a Reporting Period.
        api_response = api_instance.set_state_reporting_period_current_step(tenant_id, environment_id, reporting_period_id, ed_graph_services_state_reporting_v1_set_reporting_period_current_step_request=ed_graph_services_state_reporting_v1_set_reporting_period_current_step_request)
        print("The response of EnvironmentsReportingPeriodsApi->set_state_reporting_period_current_step:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsApi->set_state_reporting_period_current_step: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **ed_graph_services_state_reporting_v1_set_reporting_period_current_step_request** | [**EdGraphServicesStateReportingV1SetReportingPeriodCurrentStepRequest**](EdGraphServicesStateReportingV1SetReportingPeriodCurrentStepRequest.md)|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1ReportingPeriodCurrentStepSetResponse**](EdGraphServicesStateReportingV1ReportingPeriodCurrentStepSetResponse.md)

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
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**201** | The resource was created. The location of the resource is available in the Location header of the response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **set_state_reporting_period_step_status**
> EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse set_state_reporting_period_step_status(tenant_id, environment_id, reporting_period_id, step_number, ed_graph_services_state_reporting_v1_set_reporting_period_step_status_request=ed_graph_services_state_reporting_v1_set_reporting_period_step_status_request)

Sets the status of a Reporting Period step.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_created_response import EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_set_reporting_period_step_status_request import EdGraphServicesStateReportingV1SetReportingPeriodStepStatusRequest
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    step_number = 56 # int | 
    ed_graph_services_state_reporting_v1_set_reporting_period_step_status_request = edgraph_platform_client.EdGraphServicesStateReportingV1SetReportingPeriodStepStatusRequest() # EdGraphServicesStateReportingV1SetReportingPeriodStepStatusRequest |  (optional)

    try:
        # Sets the status of a Reporting Period step.
        api_response = api_instance.set_state_reporting_period_step_status(tenant_id, environment_id, reporting_period_id, step_number, ed_graph_services_state_reporting_v1_set_reporting_period_step_status_request=ed_graph_services_state_reporting_v1_set_reporting_period_step_status_request)
        print("The response of EnvironmentsReportingPeriodsApi->set_state_reporting_period_step_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsApi->set_state_reporting_period_step_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **step_number** | **int**|  | 
 **ed_graph_services_state_reporting_v1_set_reporting_period_step_status_request** | [**EdGraphServicesStateReportingV1SetReportingPeriodStepStatusRequest**](EdGraphServicesStateReportingV1SetReportingPeriodStepStatusRequest.md)|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse**](EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse.md)

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
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**201** | The resource was created. The location of the resource is available in the Location header of the response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **toggle_state_reporting_period_selected**
> EdGraphServicesStateReportingV1ReportingPeriodToggledResponse toggle_state_reporting_period_selected(tenant_id, environment_id, reporting_period_id, ed_graph_services_state_reporting_v1_toggle_reporting_period_selected_request=ed_graph_services_state_reporting_v1_toggle_reporting_period_selected_request)

Toggles the Selected state of a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_toggled_response import EdGraphServicesStateReportingV1ReportingPeriodToggledResponse
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_toggle_reporting_period_selected_request import EdGraphServicesStateReportingV1ToggleReportingPeriodSelectedRequest
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    ed_graph_services_state_reporting_v1_toggle_reporting_period_selected_request = edgraph_platform_client.EdGraphServicesStateReportingV1ToggleReportingPeriodSelectedRequest() # EdGraphServicesStateReportingV1ToggleReportingPeriodSelectedRequest |  (optional)

    try:
        # Toggles the Selected state of a Reporting Period.
        api_response = api_instance.toggle_state_reporting_period_selected(tenant_id, environment_id, reporting_period_id, ed_graph_services_state_reporting_v1_toggle_reporting_period_selected_request=ed_graph_services_state_reporting_v1_toggle_reporting_period_selected_request)
        print("The response of EnvironmentsReportingPeriodsApi->toggle_state_reporting_period_selected:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsApi->toggle_state_reporting_period_selected: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **ed_graph_services_state_reporting_v1_toggle_reporting_period_selected_request** | [**EdGraphServicesStateReportingV1ToggleReportingPeriodSelectedRequest**](EdGraphServicesStateReportingV1ToggleReportingPeriodSelectedRequest.md)|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1ReportingPeriodToggledResponse**](EdGraphServicesStateReportingV1ReportingPeriodToggledResponse.md)

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
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**201** | The resource was created. The location of the resource is available in the Location header of the response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_state_reporting_period**
> EdGraphServicesStateReportingV1ReportingPeriodUpdatedResponse update_state_reporting_period(tenant_id, environment_id, reporting_period_id, ed_graph_services_state_reporting_v1_update_reporting_period_request=ed_graph_services_state_reporting_v1_update_reporting_period_request)

Updates a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_updated_response import EdGraphServicesStateReportingV1ReportingPeriodUpdatedResponse
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_update_reporting_period_request import EdGraphServicesStateReportingV1UpdateReportingPeriodRequest
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    ed_graph_services_state_reporting_v1_update_reporting_period_request = edgraph_platform_client.EdGraphServicesStateReportingV1UpdateReportingPeriodRequest() # EdGraphServicesStateReportingV1UpdateReportingPeriodRequest |  (optional)

    try:
        # Updates a Reporting Period.
        api_response = api_instance.update_state_reporting_period(tenant_id, environment_id, reporting_period_id, ed_graph_services_state_reporting_v1_update_reporting_period_request=ed_graph_services_state_reporting_v1_update_reporting_period_request)
        print("The response of EnvironmentsReportingPeriodsApi->update_state_reporting_period:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsApi->update_state_reporting_period: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **ed_graph_services_state_reporting_v1_update_reporting_period_request** | [**EdGraphServicesStateReportingV1UpdateReportingPeriodRequest**](EdGraphServicesStateReportingV1UpdateReportingPeriodRequest.md)|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1ReportingPeriodUpdatedResponse**](EdGraphServicesStateReportingV1ReportingPeriodUpdatedResponse.md)

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
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_state_reporting_period_bulk**
> EdGraphServicesStateReportingV1ReportingPeriodUpdatedBulkResponse update_state_reporting_period_bulk(tenant_id, environment_id, ed_graph_services_state_reporting_v1_update_reporting_period_bulk_request=ed_graph_services_state_reporting_v1_update_reporting_period_bulk_request)

Updates Reporting Periods in bulk.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_updated_bulk_response import EdGraphServicesStateReportingV1ReportingPeriodUpdatedBulkResponse
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_update_reporting_period_bulk_request import EdGraphServicesStateReportingV1UpdateReportingPeriodBulkRequest
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    environment_id = 'environment_id_example' # str | 
    ed_graph_services_state_reporting_v1_update_reporting_period_bulk_request = edgraph_platform_client.EdGraphServicesStateReportingV1UpdateReportingPeriodBulkRequest() # EdGraphServicesStateReportingV1UpdateReportingPeriodBulkRequest |  (optional)

    try:
        # Updates Reporting Periods in bulk.
        api_response = api_instance.update_state_reporting_period_bulk(tenant_id, environment_id, ed_graph_services_state_reporting_v1_update_reporting_period_bulk_request=ed_graph_services_state_reporting_v1_update_reporting_period_bulk_request)
        print("The response of EnvironmentsReportingPeriodsApi->update_state_reporting_period_bulk:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsApi->update_state_reporting_period_bulk: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **environment_id** | **str**|  | 
 **ed_graph_services_state_reporting_v1_update_reporting_period_bulk_request** | [**EdGraphServicesStateReportingV1UpdateReportingPeriodBulkRequest**](EdGraphServicesStateReportingV1UpdateReportingPeriodBulkRequest.md)|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1ReportingPeriodUpdatedBulkResponse**](EdGraphServicesStateReportingV1ReportingPeriodUpdatedBulkResponse.md)

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
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

