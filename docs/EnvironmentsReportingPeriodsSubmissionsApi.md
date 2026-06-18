# edgraph_platform_client.EnvironmentsReportingPeriodsSubmissionsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_reporting_period_submission_metrics_bulk_v2**](EnvironmentsReportingPeriodsSubmissionsApi.md#add_reporting_period_submission_metrics_bulk_v2) | **POST** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/submissions/{submissionId}/metrics/bulk | Adds Metrics to a Submission in bulk.
[**add_reporting_period_submission_metrics_v2**](EnvironmentsReportingPeriodsSubmissionsApi.md#add_reporting_period_submission_metrics_v2) | **POST** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/submissions/{submissionId}/metrics | Adds Metrics to a Submission.
[**cancel_reporting_period_submission_v2**](EnvironmentsReportingPeriodsSubmissionsApi.md#cancel_reporting_period_submission_v2) | **DELETE** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/submissions/{submissionId}/cancel | Cancels a Submission.
[**get_reporting_period_submission_latest_v2**](EnvironmentsReportingPeriodsSubmissionsApi.md#get_reporting_period_submission_latest_v2) | **GET** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/submissions/latest | Retrieves the latest Submission of a Reporting Period.
[**get_reporting_period_submission_logs_v2**](EnvironmentsReportingPeriodsSubmissionsApi.md#get_reporting_period_submission_logs_v2) | **GET** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/submissions/{submissionId}/logs | Retrieves a list of Submission Logs of a Reporting Period.
[**get_reporting_period_submission_metrics_v2**](EnvironmentsReportingPeriodsSubmissionsApi.md#get_reporting_period_submission_metrics_v2) | **GET** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/submissions/{submissionId}/metrics | Retrieves the Metrics of a Submission.
[**get_reporting_period_submission_v2**](EnvironmentsReportingPeriodsSubmissionsApi.md#get_reporting_period_submission_v2) | **GET** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/submissions/{submissionId} | Retrieves the Submission of a Reporting Period.
[**get_state_reporting_period_submissions_v2**](EnvironmentsReportingPeriodsSubmissionsApi.md#get_state_reporting_period_submissions_v2) | **GET** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/submissions | Retrieves a list of Submissions of a Reporting Period.
[**set_reporting_period_submission_status_v2**](EnvironmentsReportingPeriodsSubmissionsApi.md#set_reporting_period_submission_status_v2) | **PUT** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/submissions/{submissionId}/status | Sets the Status of a Submission.


# **add_reporting_period_submission_metrics_bulk_v2**
> EdGraphServicesStateReportingV1SubmissionMetricsAddedBulkResponse add_reporting_period_submission_metrics_bulk_v2(tenant_id, environment_id, reporting_period_id, submission_id, ed_graph_services_state_reporting_v1_add_submission_metrics_bulk_request=ed_graph_services_state_reporting_v1_add_submission_metrics_bulk_request)

Adds Metrics to a Submission in bulk.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_add_submission_metrics_bulk_request import EdGraphServicesStateReportingV1AddSubmissionMetricsBulkRequest
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_submission_metrics_added_bulk_response import EdGraphServicesStateReportingV1SubmissionMetricsAddedBulkResponse
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsSubmissionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    reporting_period_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    submission_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_services_state_reporting_v1_add_submission_metrics_bulk_request = edgraph_platform_client.EdGraphServicesStateReportingV1AddSubmissionMetricsBulkRequest() # EdGraphServicesStateReportingV1AddSubmissionMetricsBulkRequest |  (optional)

    try:
        # Adds Metrics to a Submission in bulk.
        api_response = await api_instance.add_reporting_period_submission_metrics_bulk_v2(tenant_id, environment_id, reporting_period_id, submission_id, ed_graph_services_state_reporting_v1_add_submission_metrics_bulk_request=ed_graph_services_state_reporting_v1_add_submission_metrics_bulk_request)
        print("The response of EnvironmentsReportingPeriodsSubmissionsApi->add_reporting_period_submission_metrics_bulk_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsSubmissionsApi->add_reporting_period_submission_metrics_bulk_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **reporting_period_id** | **UUID**|  | 
 **submission_id** | **UUID**|  | 
 **ed_graph_services_state_reporting_v1_add_submission_metrics_bulk_request** | [**EdGraphServicesStateReportingV1AddSubmissionMetricsBulkRequest**](EdGraphServicesStateReportingV1AddSubmissionMetricsBulkRequest.md)|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1SubmissionMetricsAddedBulkResponse**](EdGraphServicesStateReportingV1SubmissionMetricsAddedBulkResponse.md)

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

# **add_reporting_period_submission_metrics_v2**
> EdGraphServicesStateReportingV1SubmissionMetricsAddedResponse add_reporting_period_submission_metrics_v2(tenant_id, environment_id, reporting_period_id, submission_id, ed_graph_services_state_reporting_v1_add_submission_metrics_request=ed_graph_services_state_reporting_v1_add_submission_metrics_request)

Adds Metrics to a Submission.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_add_submission_metrics_request import EdGraphServicesStateReportingV1AddSubmissionMetricsRequest
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_submission_metrics_added_response import EdGraphServicesStateReportingV1SubmissionMetricsAddedResponse
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsSubmissionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    reporting_period_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    submission_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_services_state_reporting_v1_add_submission_metrics_request = edgraph_platform_client.EdGraphServicesStateReportingV1AddSubmissionMetricsRequest() # EdGraphServicesStateReportingV1AddSubmissionMetricsRequest |  (optional)

    try:
        # Adds Metrics to a Submission.
        api_response = await api_instance.add_reporting_period_submission_metrics_v2(tenant_id, environment_id, reporting_period_id, submission_id, ed_graph_services_state_reporting_v1_add_submission_metrics_request=ed_graph_services_state_reporting_v1_add_submission_metrics_request)
        print("The response of EnvironmentsReportingPeriodsSubmissionsApi->add_reporting_period_submission_metrics_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsSubmissionsApi->add_reporting_period_submission_metrics_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **reporting_period_id** | **UUID**|  | 
 **submission_id** | **UUID**|  | 
 **ed_graph_services_state_reporting_v1_add_submission_metrics_request** | [**EdGraphServicesStateReportingV1AddSubmissionMetricsRequest**](EdGraphServicesStateReportingV1AddSubmissionMetricsRequest.md)|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1SubmissionMetricsAddedResponse**](EdGraphServicesStateReportingV1SubmissionMetricsAddedResponse.md)

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

# **cancel_reporting_period_submission_v2**
> EdGraphServicesStateReportingV1SubmissionCancelledResponse cancel_reporting_period_submission_v2(tenant_id, environment_id, reporting_period_id, submission_id)

Cancels a Submission.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_submission_cancelled_response import EdGraphServicesStateReportingV1SubmissionCancelledResponse
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsSubmissionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    reporting_period_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    submission_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Cancels a Submission.
        api_response = await api_instance.cancel_reporting_period_submission_v2(tenant_id, environment_id, reporting_period_id, submission_id)
        print("The response of EnvironmentsReportingPeriodsSubmissionsApi->cancel_reporting_period_submission_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsSubmissionsApi->cancel_reporting_period_submission_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **reporting_period_id** | **UUID**|  | 
 **submission_id** | **UUID**|  | 

### Return type

[**EdGraphServicesStateReportingV1SubmissionCancelledResponse**](EdGraphServicesStateReportingV1SubmissionCancelledResponse.md)

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_reporting_period_submission_latest_v2**
> EdGraphServicesStateReportingV1SubmissionProfile get_reporting_period_submission_latest_v2(tenant_id, environment_id, reporting_period_id)

Retrieves the latest Submission of a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_submission_profile import EdGraphServicesStateReportingV1SubmissionProfile
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsSubmissionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    reporting_period_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Retrieves the latest Submission of a Reporting Period.
        api_response = await api_instance.get_reporting_period_submission_latest_v2(tenant_id, environment_id, reporting_period_id)
        print("The response of EnvironmentsReportingPeriodsSubmissionsApi->get_reporting_period_submission_latest_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsSubmissionsApi->get_reporting_period_submission_latest_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **reporting_period_id** | **UUID**|  | 

### Return type

[**EdGraphServicesStateReportingV1SubmissionProfile**](EdGraphServicesStateReportingV1SubmissionProfile.md)

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

# **get_reporting_period_submission_logs_v2**
> EdGraphServicesStateReportingV1PaginatedSubmissionLogs get_reporting_period_submission_logs_v2(tenant_id, environment_id, reporting_period_id, submission_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)

Retrieves a list of Submission Logs of a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_paginated_submission_logs import EdGraphServicesStateReportingV1PaginatedSubmissionLogs
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsSubmissionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    reporting_period_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    submission_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_index = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    filter = 'filter_example' # str |  (optional)
    order_by = 'order_by_example' # str |  (optional)

    try:
        # Retrieves a list of Submission Logs of a Reporting Period.
        api_response = await api_instance.get_reporting_period_submission_logs_v2(tenant_id, environment_id, reporting_period_id, submission_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)
        print("The response of EnvironmentsReportingPeriodsSubmissionsApi->get_reporting_period_submission_logs_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsSubmissionsApi->get_reporting_period_submission_logs_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **reporting_period_id** | **UUID**|  | 
 **submission_id** | **UUID**|  | 
 **page_index** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **filter** | **str**|  | [optional] 
 **order_by** | **str**|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1PaginatedSubmissionLogs**](EdGraphServicesStateReportingV1PaginatedSubmissionLogs.md)

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

# **get_reporting_period_submission_metrics_v2**
> EdGraphServicesStateReportingV1SubmissionMetricsResponse get_reporting_period_submission_metrics_v2(tenant_id, environment_id, reporting_period_id, submission_id)

Retrieves the Metrics of a Submission.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_submission_metrics_response import EdGraphServicesStateReportingV1SubmissionMetricsResponse
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsSubmissionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    reporting_period_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    submission_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Retrieves the Metrics of a Submission.
        api_response = await api_instance.get_reporting_period_submission_metrics_v2(tenant_id, environment_id, reporting_period_id, submission_id)
        print("The response of EnvironmentsReportingPeriodsSubmissionsApi->get_reporting_period_submission_metrics_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsSubmissionsApi->get_reporting_period_submission_metrics_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **reporting_period_id** | **UUID**|  | 
 **submission_id** | **UUID**|  | 

### Return type

[**EdGraphServicesStateReportingV1SubmissionMetricsResponse**](EdGraphServicesStateReportingV1SubmissionMetricsResponse.md)

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

# **get_reporting_period_submission_v2**
> EdGraphServicesStateReportingV1SubmissionProfile get_reporting_period_submission_v2(tenant_id, environment_id, reporting_period_id, submission_id)

Retrieves the Submission of a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_submission_profile import EdGraphServicesStateReportingV1SubmissionProfile
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsSubmissionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    reporting_period_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    submission_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Retrieves the Submission of a Reporting Period.
        api_response = await api_instance.get_reporting_period_submission_v2(tenant_id, environment_id, reporting_period_id, submission_id)
        print("The response of EnvironmentsReportingPeriodsSubmissionsApi->get_reporting_period_submission_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsSubmissionsApi->get_reporting_period_submission_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **reporting_period_id** | **UUID**|  | 
 **submission_id** | **UUID**|  | 

### Return type

[**EdGraphServicesStateReportingV1SubmissionProfile**](EdGraphServicesStateReportingV1SubmissionProfile.md)

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

# **get_state_reporting_period_submissions_v2**
> EdGraphServicesStateReportingV1PaginatedSubmissions get_state_reporting_period_submissions_v2(tenant_id, environment_id, reporting_period_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)

Retrieves a list of Submissions of a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_paginated_submissions import EdGraphServicesStateReportingV1PaginatedSubmissions
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsSubmissionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    reporting_period_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    filter = '' # str |  (optional) (default to '')
    order_by = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of Submissions of a Reporting Period.
        api_response = await api_instance.get_state_reporting_period_submissions_v2(tenant_id, environment_id, reporting_period_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)
        print("The response of EnvironmentsReportingPeriodsSubmissionsApi->get_state_reporting_period_submissions_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsSubmissionsApi->get_state_reporting_period_submissions_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **reporting_period_id** | **UUID**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphServicesStateReportingV1PaginatedSubmissions**](EdGraphServicesStateReportingV1PaginatedSubmissions.md)

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

# **set_reporting_period_submission_status_v2**
> EdGraphServicesStateReportingV1SubmissionStatusSetResponse set_reporting_period_submission_status_v2(tenant_id, environment_id, reporting_period_id, submission_id, ed_graph_services_state_reporting_v1_set_submission_status_request=ed_graph_services_state_reporting_v1_set_submission_status_request)

Sets the Status of a Submission.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_set_submission_status_request import EdGraphServicesStateReportingV1SetSubmissionStatusRequest
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_submission_status_set_response import EdGraphServicesStateReportingV1SubmissionStatusSetResponse
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsSubmissionsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    reporting_period_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    submission_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_services_state_reporting_v1_set_submission_status_request = edgraph_platform_client.EdGraphServicesStateReportingV1SetSubmissionStatusRequest() # EdGraphServicesStateReportingV1SetSubmissionStatusRequest |  (optional)

    try:
        # Sets the Status of a Submission.
        api_response = await api_instance.set_reporting_period_submission_status_v2(tenant_id, environment_id, reporting_period_id, submission_id, ed_graph_services_state_reporting_v1_set_submission_status_request=ed_graph_services_state_reporting_v1_set_submission_status_request)
        print("The response of EnvironmentsReportingPeriodsSubmissionsApi->set_reporting_period_submission_status_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsSubmissionsApi->set_reporting_period_submission_status_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **reporting_period_id** | **UUID**|  | 
 **submission_id** | **UUID**|  | 
 **ed_graph_services_state_reporting_v1_set_submission_status_request** | [**EdGraphServicesStateReportingV1SetSubmissionStatusRequest**](EdGraphServicesStateReportingV1SetSubmissionStatusRequest.md)|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1SubmissionStatusSetResponse**](EdGraphServicesStateReportingV1SubmissionStatusSetResponse.md)

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

