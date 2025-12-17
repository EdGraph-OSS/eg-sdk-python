# edgraph_platform_client.ReportingPeriodsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_reporting_period_submission_metrics**](ReportingPeriodsApi.md#add_reporting_period_submission_metrics) | **POST** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/submissions/{submissionId}/metrics | Adds Metrics to a Submission.
[**add_reporting_period_submission_metrics_bulk**](ReportingPeriodsApi.md#add_reporting_period_submission_metrics_bulk) | **POST** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/submissions/{submissionId}/metrics/bulk | Adds Metrics to a Submission in bulk.
[**cancel_reporting_period_submission**](ReportingPeriodsApi.md#cancel_reporting_period_submission) | **DELETE** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/submissions/{submissionId}/cancel | Cancels a Submission.
[**close_reporting_period_async**](ReportingPeriodsApi.md#close_reporting_period_async) | **PUT** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/close | Closes the state of a Reporting Period.
[**delete_reporting_period_rules**](ReportingPeriodsApi.md#delete_reporting_period_rules) | **DELETE** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/rules | Delete the Reporting Period and Associated Rules
[**get_reporting_period_certification_status**](ReportingPeriodsApi.md#get_reporting_period_certification_status) | **GET** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/certificationstatus | Retrieves the Certification Status of a Reporting Period.
[**get_reporting_period_records**](ReportingPeriodsApi.md#get_reporting_period_records) | **GET** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/records | Retrieves the Invalid Records of all the Rules within a Reporting Period.
[**get_reporting_period_rule_records**](ReportingPeriodsApi.md#get_reporting_period_rule_records) | **GET** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/rules/{ruleId}/records | Retrieves the Invalid Records of a Rule.
[**get_reporting_period_submission**](ReportingPeriodsApi.md#get_reporting_period_submission) | **GET** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/submissions/{submissionId} | Retrieves the Submission of a Reporting Period.
[**get_reporting_period_submission_latest**](ReportingPeriodsApi.md#get_reporting_period_submission_latest) | **GET** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/submissions/latest | Retrieves the latest Submission of a Reporting Period.
[**get_reporting_period_submission_logs**](ReportingPeriodsApi.md#get_reporting_period_submission_logs) | **GET** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/submissions/{submissionId}/logs | Retrieves a list of Submission Logs of a Reporting Period.
[**get_reporting_period_submission_metrics**](ReportingPeriodsApi.md#get_reporting_period_submission_metrics) | **GET** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/submissions/{submissionId}/metrics | Retrieves the Metrics of a Submission.
[**get_reporting_period_submissions**](ReportingPeriodsApi.md#get_reporting_period_submissions) | **GET** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/submissions | Retrieves a list of Submissions of a Reporting Period.
[**get_reporting_period_validation_summary**](ReportingPeriodsApi.md#get_reporting_period_validation_summary) | **GET** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/validationsummary | Retrieves the Validation Summary of a Reporting Period.
[**get_reporting_period_validation_summary_by_category_id**](ReportingPeriodsApi.md#get_reporting_period_validation_summary_by_category_id) | **GET** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/validationsummary/categories/{categoryId} | Retrieves the Validation Summary of a Reporting Period for a Category.
[**get_reporting_periods**](ReportingPeriodsApi.md#get_reporting_periods) | **GET** /tenants/{tenantId}/statereporting/reportingperiods | Retrieves a list of Reporting Periods.
[**post_reporting_period**](ReportingPeriodsApi.md#post_reporting_period) | **POST** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/post | Post a Reporting Period.
[**run_reporting_period_validations**](ReportingPeriodsApi.md#run_reporting_period_validations) | **POST** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/run | Run Reporting Period Validations.
[**set_reporting_period_rule_record_exclude_from_post_flag_bulk**](ReportingPeriodsApi.md#set_reporting_period_rule_record_exclude_from_post_flag_bulk) | **PUT** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/rules/{ruleId}/records/excludefrompost | Toggles the \&quot;ExcludeFromPost\&quot; flag of a Rule&#39;s Invalid Records.
[**set_reporting_period_submission_status**](ReportingPeriodsApi.md#set_reporting_period_submission_status) | **PUT** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/submissions/{submissionId}/status | Sets the Status of a Submission.
[**toggle_reporting_period_selection**](ReportingPeriodsApi.md#toggle_reporting_period_selection) | **PUT** /tenants/{tenantId}/statereporting/reportingperiods/{reportingPeriodId}/toggle | Toggles the Selected state of a Reporting Period.
[**update_reporting_period_bulk**](ReportingPeriodsApi.md#update_reporting_period_bulk) | **PUT** /tenants/{tenantId}/statereporting/reportingperiods | Updates Reporting Periods in bulk.


# **add_reporting_period_submission_metrics**
> ValidationsApiReportingPeriodsV1SubmissionMetricsAddedResponse add_reporting_period_submission_metrics(tenant_id, reporting_period_id, submission_id, validations_api_reporting_periods_v1_add_submission_metrics_request=validations_api_reporting_periods_v1_add_submission_metrics_request)

Adds Metrics to a Submission.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_add_submission_metrics_request import ValidationsApiReportingPeriodsV1AddSubmissionMetricsRequest
from edgraph_platform_client.models.validations_api_reporting_periods_v1_submission_metrics_added_response import ValidationsApiReportingPeriodsV1SubmissionMetricsAddedResponse
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    submission_id = 'submission_id_example' # str | 
    validations_api_reporting_periods_v1_add_submission_metrics_request = edgraph_platform_client.ValidationsApiReportingPeriodsV1AddSubmissionMetricsRequest() # ValidationsApiReportingPeriodsV1AddSubmissionMetricsRequest |  (optional)

    try:
        # Adds Metrics to a Submission.
        api_response = api_instance.add_reporting_period_submission_metrics(tenant_id, reporting_period_id, submission_id, validations_api_reporting_periods_v1_add_submission_metrics_request=validations_api_reporting_periods_v1_add_submission_metrics_request)
        print("The response of ReportingPeriodsApi->add_reporting_period_submission_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->add_reporting_period_submission_metrics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **submission_id** | **str**|  | 
 **validations_api_reporting_periods_v1_add_submission_metrics_request** | [**ValidationsApiReportingPeriodsV1AddSubmissionMetricsRequest**](ValidationsApiReportingPeriodsV1AddSubmissionMetricsRequest.md)|  | [optional] 

### Return type

[**ValidationsApiReportingPeriodsV1SubmissionMetricsAddedResponse**](ValidationsApiReportingPeriodsV1SubmissionMetricsAddedResponse.md)

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

# **add_reporting_period_submission_metrics_bulk**
> ValidationsApiReportingPeriodsV1SubmissionMetricsAddedBulkResponse add_reporting_period_submission_metrics_bulk(tenant_id, reporting_period_id, submission_id, validations_api_reporting_periods_v1_add_submission_metrics_bulk_request=validations_api_reporting_periods_v1_add_submission_metrics_bulk_request)

Adds Metrics to a Submission in bulk.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_add_submission_metrics_bulk_request import ValidationsApiReportingPeriodsV1AddSubmissionMetricsBulkRequest
from edgraph_platform_client.models.validations_api_reporting_periods_v1_submission_metrics_added_bulk_response import ValidationsApiReportingPeriodsV1SubmissionMetricsAddedBulkResponse
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    submission_id = 'submission_id_example' # str | 
    validations_api_reporting_periods_v1_add_submission_metrics_bulk_request = edgraph_platform_client.ValidationsApiReportingPeriodsV1AddSubmissionMetricsBulkRequest() # ValidationsApiReportingPeriodsV1AddSubmissionMetricsBulkRequest |  (optional)

    try:
        # Adds Metrics to a Submission in bulk.
        api_response = api_instance.add_reporting_period_submission_metrics_bulk(tenant_id, reporting_period_id, submission_id, validations_api_reporting_periods_v1_add_submission_metrics_bulk_request=validations_api_reporting_periods_v1_add_submission_metrics_bulk_request)
        print("The response of ReportingPeriodsApi->add_reporting_period_submission_metrics_bulk:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->add_reporting_period_submission_metrics_bulk: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **submission_id** | **str**|  | 
 **validations_api_reporting_periods_v1_add_submission_metrics_bulk_request** | [**ValidationsApiReportingPeriodsV1AddSubmissionMetricsBulkRequest**](ValidationsApiReportingPeriodsV1AddSubmissionMetricsBulkRequest.md)|  | [optional] 

### Return type

[**ValidationsApiReportingPeriodsV1SubmissionMetricsAddedBulkResponse**](ValidationsApiReportingPeriodsV1SubmissionMetricsAddedBulkResponse.md)

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

# **cancel_reporting_period_submission**
> ValidationsApiReportingPeriodsV1SubmissionCancelledResponse cancel_reporting_period_submission(tenant_id, reporting_period_id, submission_id)

Cancels a Submission.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_submission_cancelled_response import ValidationsApiReportingPeriodsV1SubmissionCancelledResponse
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    submission_id = 'submission_id_example' # str | 

    try:
        # Cancels a Submission.
        api_response = api_instance.cancel_reporting_period_submission(tenant_id, reporting_period_id, submission_id)
        print("The response of ReportingPeriodsApi->cancel_reporting_period_submission:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->cancel_reporting_period_submission: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **submission_id** | **str**|  | 

### Return type

[**ValidationsApiReportingPeriodsV1SubmissionCancelledResponse**](ValidationsApiReportingPeriodsV1SubmissionCancelledResponse.md)

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

# **close_reporting_period_async**
> ValidationsApiReportingPeriodsV1CloseReportingPeriodResponse close_reporting_period_async(tenant_id, reporting_period_id)

Closes the state of a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_close_reporting_period_response import ValidationsApiReportingPeriodsV1CloseReportingPeriodResponse
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 

    try:
        # Closes the state of a Reporting Period.
        api_response = api_instance.close_reporting_period_async(tenant_id, reporting_period_id)
        print("The response of ReportingPeriodsApi->close_reporting_period_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->close_reporting_period_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 

### Return type

[**ValidationsApiReportingPeriodsV1CloseReportingPeriodResponse**](ValidationsApiReportingPeriodsV1CloseReportingPeriodResponse.md)

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

# **delete_reporting_period_rules**
> ValidationsApiReportingPeriodsV1DeleteReportingPeriodRulesResponse delete_reporting_period_rules(tenant_id, reporting_period_id)

Delete the Reporting Period and Associated Rules

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_delete_reporting_period_rules_response import ValidationsApiReportingPeriodsV1DeleteReportingPeriodRulesResponse
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 

    try:
        # Delete the Reporting Period and Associated Rules
        api_response = api_instance.delete_reporting_period_rules(tenant_id, reporting_period_id)
        print("The response of ReportingPeriodsApi->delete_reporting_period_rules:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->delete_reporting_period_rules: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 

### Return type

[**ValidationsApiReportingPeriodsV1DeleteReportingPeriodRulesResponse**](ValidationsApiReportingPeriodsV1DeleteReportingPeriodRulesResponse.md)

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

# **get_reporting_period_certification_status**
> ValidationsApiReportingPeriodsV1CertificationStatus get_reporting_period_certification_status(tenant_id, reporting_period_id)

Retrieves the Certification Status of a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_certification_status import ValidationsApiReportingPeriodsV1CertificationStatus
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 

    try:
        # Retrieves the Certification Status of a Reporting Period.
        api_response = api_instance.get_reporting_period_certification_status(tenant_id, reporting_period_id)
        print("The response of ReportingPeriodsApi->get_reporting_period_certification_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->get_reporting_period_certification_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 

### Return type

[**ValidationsApiReportingPeriodsV1CertificationStatus**](ValidationsApiReportingPeriodsV1CertificationStatus.md)

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

# **get_reporting_period_records**
> ValidationsApiReportingPeriodsV1PaginatedRecords get_reporting_period_records(tenant_id, reporting_period_id, page_index=page_index, page_size=page_size, excluded_from_post=excluded_from_post)

Retrieves the Invalid Records of all the Rules within a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_paginated_records import ValidationsApiReportingPeriodsV1PaginatedRecords
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    excluded_from_post = True # bool |  (optional)

    try:
        # Retrieves the Invalid Records of all the Rules within a Reporting Period.
        api_response = api_instance.get_reporting_period_records(tenant_id, reporting_period_id, page_index=page_index, page_size=page_size, excluded_from_post=excluded_from_post)
        print("The response of ReportingPeriodsApi->get_reporting_period_records:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->get_reporting_period_records: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **excluded_from_post** | **bool**|  | [optional] 

### Return type

[**ValidationsApiReportingPeriodsV1PaginatedRecords**](ValidationsApiReportingPeriodsV1PaginatedRecords.md)

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

# **get_reporting_period_rule_records**
> ValidationsApiReportingPeriodsV1PaginatedRuleRecordsV2 get_reporting_period_rule_records(tenant_id, reporting_period_id, rule_id, page_index=page_index, page_size=page_size)

Retrieves the Invalid Records of a Rule.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_paginated_rule_records_v2 import ValidationsApiReportingPeriodsV1PaginatedRuleRecordsV2
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    rule_id = 'rule_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)

    try:
        # Retrieves the Invalid Records of a Rule.
        api_response = api_instance.get_reporting_period_rule_records(tenant_id, reporting_period_id, rule_id, page_index=page_index, page_size=page_size)
        print("The response of ReportingPeriodsApi->get_reporting_period_rule_records:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->get_reporting_period_rule_records: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **rule_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]

### Return type

[**ValidationsApiReportingPeriodsV1PaginatedRuleRecordsV2**](ValidationsApiReportingPeriodsV1PaginatedRuleRecordsV2.md)

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

# **get_reporting_period_submission**
> ValidationsApiReportingPeriodsV1SubmissionProfile get_reporting_period_submission(tenant_id, reporting_period_id, submission_id)

Retrieves the Submission of a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_submission_profile import ValidationsApiReportingPeriodsV1SubmissionProfile
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    submission_id = 'submission_id_example' # str | 

    try:
        # Retrieves the Submission of a Reporting Period.
        api_response = api_instance.get_reporting_period_submission(tenant_id, reporting_period_id, submission_id)
        print("The response of ReportingPeriodsApi->get_reporting_period_submission:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->get_reporting_period_submission: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **submission_id** | **str**|  | 

### Return type

[**ValidationsApiReportingPeriodsV1SubmissionProfile**](ValidationsApiReportingPeriodsV1SubmissionProfile.md)

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

# **get_reporting_period_submission_latest**
> ValidationsApiReportingPeriodsV1SubmissionProfile get_reporting_period_submission_latest(tenant_id, reporting_period_id)

Retrieves the latest Submission of a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_submission_profile import ValidationsApiReportingPeriodsV1SubmissionProfile
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 

    try:
        # Retrieves the latest Submission of a Reporting Period.
        api_response = api_instance.get_reporting_period_submission_latest(tenant_id, reporting_period_id)
        print("The response of ReportingPeriodsApi->get_reporting_period_submission_latest:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->get_reporting_period_submission_latest: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 

### Return type

[**ValidationsApiReportingPeriodsV1SubmissionProfile**](ValidationsApiReportingPeriodsV1SubmissionProfile.md)

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

# **get_reporting_period_submission_logs**
> ValidationsApiReportingPeriodsV1PaginatedSubmissions get_reporting_period_submission_logs(tenant_id, reporting_period_id, submission_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)

Retrieves a list of Submission Logs of a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_paginated_submissions import ValidationsApiReportingPeriodsV1PaginatedSubmissions
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    submission_id = 'submission_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    filter = '' # str |  (optional) (default to '')
    order_by = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of Submission Logs of a Reporting Period.
        api_response = api_instance.get_reporting_period_submission_logs(tenant_id, reporting_period_id, submission_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)
        print("The response of ReportingPeriodsApi->get_reporting_period_submission_logs:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->get_reporting_period_submission_logs: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **submission_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**ValidationsApiReportingPeriodsV1PaginatedSubmissions**](ValidationsApiReportingPeriodsV1PaginatedSubmissions.md)

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

# **get_reporting_period_submission_metrics**
> ValidationsApiReportingPeriodsV1SubmissionMetricsResponse get_reporting_period_submission_metrics(tenant_id, reporting_period_id, submission_id)

Retrieves the Metrics of a Submission.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_submission_metrics_response import ValidationsApiReportingPeriodsV1SubmissionMetricsResponse
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    submission_id = 'submission_id_example' # str | 

    try:
        # Retrieves the Metrics of a Submission.
        api_response = api_instance.get_reporting_period_submission_metrics(tenant_id, reporting_period_id, submission_id)
        print("The response of ReportingPeriodsApi->get_reporting_period_submission_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->get_reporting_period_submission_metrics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **submission_id** | **str**|  | 

### Return type

[**ValidationsApiReportingPeriodsV1SubmissionMetricsResponse**](ValidationsApiReportingPeriodsV1SubmissionMetricsResponse.md)

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

# **get_reporting_period_submissions**
> ValidationsApiReportingPeriodsV1PaginatedSubmissions get_reporting_period_submissions(tenant_id, reporting_period_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)

Retrieves a list of Submissions of a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_paginated_submissions import ValidationsApiReportingPeriodsV1PaginatedSubmissions
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    filter = '' # str |  (optional) (default to '')
    order_by = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of Submissions of a Reporting Period.
        api_response = api_instance.get_reporting_period_submissions(tenant_id, reporting_period_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)
        print("The response of ReportingPeriodsApi->get_reporting_period_submissions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->get_reporting_period_submissions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**ValidationsApiReportingPeriodsV1PaginatedSubmissions**](ValidationsApiReportingPeriodsV1PaginatedSubmissions.md)

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

# **get_reporting_period_validation_summary**
> ValidationsApiReportingPeriodsV1ValidationSummary get_reporting_period_validation_summary(tenant_id, reporting_period_id)

Retrieves the Validation Summary of a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_validation_summary import ValidationsApiReportingPeriodsV1ValidationSummary
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 

    try:
        # Retrieves the Validation Summary of a Reporting Period.
        api_response = api_instance.get_reporting_period_validation_summary(tenant_id, reporting_period_id)
        print("The response of ReportingPeriodsApi->get_reporting_period_validation_summary:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->get_reporting_period_validation_summary: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 

### Return type

[**ValidationsApiReportingPeriodsV1ValidationSummary**](ValidationsApiReportingPeriodsV1ValidationSummary.md)

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

# **get_reporting_period_validation_summary_by_category_id**
> ValidationsApiReportingPeriodsV1ValidationSummaryByCategoryId get_reporting_period_validation_summary_by_category_id(tenant_id, reporting_period_id, category_id)

Retrieves the Validation Summary of a Reporting Period for a Category.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_validation_summary_by_category_id import ValidationsApiReportingPeriodsV1ValidationSummaryByCategoryId
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    category_id = 'category_id_example' # str | 

    try:
        # Retrieves the Validation Summary of a Reporting Period for a Category.
        api_response = api_instance.get_reporting_period_validation_summary_by_category_id(tenant_id, reporting_period_id, category_id)
        print("The response of ReportingPeriodsApi->get_reporting_period_validation_summary_by_category_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->get_reporting_period_validation_summary_by_category_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **category_id** | **str**|  | 

### Return type

[**ValidationsApiReportingPeriodsV1ValidationSummaryByCategoryId**](ValidationsApiReportingPeriodsV1ValidationSummaryByCategoryId.md)

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

# **get_reporting_periods**
> ValidationsApiReportingPeriodsV1PaginatedReportingPeriods get_reporting_periods(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)

Retrieves a list of Reporting Periods.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_paginated_reporting_periods import ValidationsApiReportingPeriodsV1PaginatedReportingPeriods
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    filter = '' # str |  (optional) (default to '')
    order_by = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of Reporting Periods.
        api_response = api_instance.get_reporting_periods(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)
        print("The response of ReportingPeriodsApi->get_reporting_periods:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->get_reporting_periods: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**ValidationsApiReportingPeriodsV1PaginatedReportingPeriods**](ValidationsApiReportingPeriodsV1PaginatedReportingPeriods.md)

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

# **post_reporting_period**
> ValidationsApiReportingPeriodsV1PostedResponse post_reporting_period(tenant_id, reporting_period_id, validations_api_reporting_periods_v1_post_request=validations_api_reporting_periods_v1_post_request)

Post a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_post_request import ValidationsApiReportingPeriodsV1PostRequest
from edgraph_platform_client.models.validations_api_reporting_periods_v1_posted_response import ValidationsApiReportingPeriodsV1PostedResponse
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    validations_api_reporting_periods_v1_post_request = edgraph_platform_client.ValidationsApiReportingPeriodsV1PostRequest() # ValidationsApiReportingPeriodsV1PostRequest |  (optional)

    try:
        # Post a Reporting Period.
        api_response = api_instance.post_reporting_period(tenant_id, reporting_period_id, validations_api_reporting_periods_v1_post_request=validations_api_reporting_periods_v1_post_request)
        print("The response of ReportingPeriodsApi->post_reporting_period:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->post_reporting_period: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **validations_api_reporting_periods_v1_post_request** | [**ValidationsApiReportingPeriodsV1PostRequest**](ValidationsApiReportingPeriodsV1PostRequest.md)|  | [optional] 

### Return type

[**ValidationsApiReportingPeriodsV1PostedResponse**](ValidationsApiReportingPeriodsV1PostedResponse.md)

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

# **run_reporting_period_validations**
> ValidationsApiReportingPeriodsV1RunResponse run_reporting_period_validations(tenant_id, reporting_period_id, category_id=category_id)

Run Reporting Period Validations.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_run_response import ValidationsApiReportingPeriodsV1RunResponse
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    category_id = 'category_id_example' # str |  (optional)

    try:
        # Run Reporting Period Validations.
        api_response = api_instance.run_reporting_period_validations(tenant_id, reporting_period_id, category_id=category_id)
        print("The response of ReportingPeriodsApi->run_reporting_period_validations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->run_reporting_period_validations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **category_id** | **str**|  | [optional] 

### Return type

[**ValidationsApiReportingPeriodsV1RunResponse**](ValidationsApiReportingPeriodsV1RunResponse.md)

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

# **set_reporting_period_rule_record_exclude_from_post_flag_bulk**
> ValidationsApiReportingPeriodsV1RuleRecordPostFlagSetBulkResponse set_reporting_period_rule_record_exclude_from_post_flag_bulk(tenant_id, reporting_period_id, rule_id, validations_api_reporting_periods_v1_set_rule_record_post_flag_bulk_request=validations_api_reporting_periods_v1_set_rule_record_post_flag_bulk_request)

Toggles the \"ExcludeFromPost\" flag of a Rule's Invalid Records.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_rule_record_post_flag_set_bulk_response import ValidationsApiReportingPeriodsV1RuleRecordPostFlagSetBulkResponse
from edgraph_platform_client.models.validations_api_reporting_periods_v1_set_rule_record_post_flag_bulk_request import ValidationsApiReportingPeriodsV1SetRuleRecordPostFlagBulkRequest
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    rule_id = 'rule_id_example' # str | 
    validations_api_reporting_periods_v1_set_rule_record_post_flag_bulk_request = edgraph_platform_client.ValidationsApiReportingPeriodsV1SetRuleRecordPostFlagBulkRequest() # ValidationsApiReportingPeriodsV1SetRuleRecordPostFlagBulkRequest |  (optional)

    try:
        # Toggles the \"ExcludeFromPost\" flag of a Rule's Invalid Records.
        api_response = api_instance.set_reporting_period_rule_record_exclude_from_post_flag_bulk(tenant_id, reporting_period_id, rule_id, validations_api_reporting_periods_v1_set_rule_record_post_flag_bulk_request=validations_api_reporting_periods_v1_set_rule_record_post_flag_bulk_request)
        print("The response of ReportingPeriodsApi->set_reporting_period_rule_record_exclude_from_post_flag_bulk:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->set_reporting_period_rule_record_exclude_from_post_flag_bulk: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **rule_id** | **str**|  | 
 **validations_api_reporting_periods_v1_set_rule_record_post_flag_bulk_request** | [**ValidationsApiReportingPeriodsV1SetRuleRecordPostFlagBulkRequest**](ValidationsApiReportingPeriodsV1SetRuleRecordPostFlagBulkRequest.md)|  | [optional] 

### Return type

[**ValidationsApiReportingPeriodsV1RuleRecordPostFlagSetBulkResponse**](ValidationsApiReportingPeriodsV1RuleRecordPostFlagSetBulkResponse.md)

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

# **set_reporting_period_submission_status**
> ValidationsApiReportingPeriodsV1SubmissionStatusSetResponse set_reporting_period_submission_status(tenant_id, reporting_period_id, submission_id, validations_api_reporting_periods_v1_set_submission_status_request=validations_api_reporting_periods_v1_set_submission_status_request)

Sets the Status of a Submission.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_set_submission_status_request import ValidationsApiReportingPeriodsV1SetSubmissionStatusRequest
from edgraph_platform_client.models.validations_api_reporting_periods_v1_submission_status_set_response import ValidationsApiReportingPeriodsV1SubmissionStatusSetResponse
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    submission_id = 'submission_id_example' # str | 
    validations_api_reporting_periods_v1_set_submission_status_request = edgraph_platform_client.ValidationsApiReportingPeriodsV1SetSubmissionStatusRequest() # ValidationsApiReportingPeriodsV1SetSubmissionStatusRequest |  (optional)

    try:
        # Sets the Status of a Submission.
        api_response = api_instance.set_reporting_period_submission_status(tenant_id, reporting_period_id, submission_id, validations_api_reporting_periods_v1_set_submission_status_request=validations_api_reporting_periods_v1_set_submission_status_request)
        print("The response of ReportingPeriodsApi->set_reporting_period_submission_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->set_reporting_period_submission_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **submission_id** | **str**|  | 
 **validations_api_reporting_periods_v1_set_submission_status_request** | [**ValidationsApiReportingPeriodsV1SetSubmissionStatusRequest**](ValidationsApiReportingPeriodsV1SetSubmissionStatusRequest.md)|  | [optional] 

### Return type

[**ValidationsApiReportingPeriodsV1SubmissionStatusSetResponse**](ValidationsApiReportingPeriodsV1SubmissionStatusSetResponse.md)

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

# **toggle_reporting_period_selection**
> ValidationsApiReportingPeriodsV1ToggledResponse toggle_reporting_period_selection(tenant_id, reporting_period_id, validations_api_reporting_periods_v1_toggle_selected_request=validations_api_reporting_periods_v1_toggle_selected_request)

Toggles the Selected state of a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_toggle_selected_request import ValidationsApiReportingPeriodsV1ToggleSelectedRequest
from edgraph_platform_client.models.validations_api_reporting_periods_v1_toggled_response import ValidationsApiReportingPeriodsV1ToggledResponse
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    reporting_period_id = 'reporting_period_id_example' # str | 
    validations_api_reporting_periods_v1_toggle_selected_request = edgraph_platform_client.ValidationsApiReportingPeriodsV1ToggleSelectedRequest() # ValidationsApiReportingPeriodsV1ToggleSelectedRequest |  (optional)

    try:
        # Toggles the Selected state of a Reporting Period.
        api_response = api_instance.toggle_reporting_period_selection(tenant_id, reporting_period_id, validations_api_reporting_periods_v1_toggle_selected_request=validations_api_reporting_periods_v1_toggle_selected_request)
        print("The response of ReportingPeriodsApi->toggle_reporting_period_selection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->toggle_reporting_period_selection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **reporting_period_id** | **str**|  | 
 **validations_api_reporting_periods_v1_toggle_selected_request** | [**ValidationsApiReportingPeriodsV1ToggleSelectedRequest**](ValidationsApiReportingPeriodsV1ToggleSelectedRequest.md)|  | [optional] 

### Return type

[**ValidationsApiReportingPeriodsV1ToggledResponse**](ValidationsApiReportingPeriodsV1ToggledResponse.md)

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

# **update_reporting_period_bulk**
> ValidationsApiReportingPeriodsV1UpdatedBulkResponse update_reporting_period_bulk(tenant_id, validations_api_reporting_periods_v1_update_bulk_request=validations_api_reporting_periods_v1_update_bulk_request)

Updates Reporting Periods in bulk.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_reporting_periods_v1_update_bulk_request import ValidationsApiReportingPeriodsV1UpdateBulkRequest
from edgraph_platform_client.models.validations_api_reporting_periods_v1_updated_bulk_response import ValidationsApiReportingPeriodsV1UpdatedBulkResponse
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
    api_instance = edgraph_platform_client.ReportingPeriodsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    validations_api_reporting_periods_v1_update_bulk_request = edgraph_platform_client.ValidationsApiReportingPeriodsV1UpdateBulkRequest() # ValidationsApiReportingPeriodsV1UpdateBulkRequest |  (optional)

    try:
        # Updates Reporting Periods in bulk.
        api_response = api_instance.update_reporting_period_bulk(tenant_id, validations_api_reporting_periods_v1_update_bulk_request=validations_api_reporting_periods_v1_update_bulk_request)
        print("The response of ReportingPeriodsApi->update_reporting_period_bulk:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportingPeriodsApi->update_reporting_period_bulk: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **validations_api_reporting_periods_v1_update_bulk_request** | [**ValidationsApiReportingPeriodsV1UpdateBulkRequest**](ValidationsApiReportingPeriodsV1UpdateBulkRequest.md)|  | [optional] 

### Return type

[**ValidationsApiReportingPeriodsV1UpdatedBulkResponse**](ValidationsApiReportingPeriodsV1UpdatedBulkResponse.md)

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

