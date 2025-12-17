# edgraph_platform_client.ValidationResultsAPIApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**find_results_api_job_run_records_async**](ValidationResultsAPIApi.md#find_results_api_job_run_records_async) | **GET** /tenants/{tenantId}/validations/results-api/jobs/{jobId}/runs/{runId}/records | Retrieves a list of Job Run Records from the Validation Results API.
[**find_results_api_job_run_rule_records_async**](ValidationResultsAPIApi.md#find_results_api_job_run_rule_records_async) | **GET** /tenants/{tenantId}/validations/results-api/jobs/{jobId}/runs/{runId}/rules/{ruleId}/records | Retrieves a list of Job Run Rule Records from the Validation Results API.
[**find_results_api_job_run_rules_async**](ValidationResultsAPIApi.md#find_results_api_job_run_rules_async) | **GET** /tenants/{tenantId}/validations/results-api/jobs/{jobId}/runs/{runId}/rules | Retrieves a list of Job Run Rules from the Validation Results API.
[**find_results_api_job_runs_async**](ValidationResultsAPIApi.md#find_results_api_job_runs_async) | **GET** /tenants/{tenantId}/validations/results-api/jobs/{jobId}/runs | Retrieves a list of Job Runs from the Validation Results API.
[**find_results_api_jobs_async**](ValidationResultsAPIApi.md#find_results_api_jobs_async) | **GET** /tenants/{tenantId}/validations/results-api/jobs | Retrieves a list of Jobs from the Validation Results API.
[**find_results_api_rule_summaries**](ValidationResultsAPIApi.md#find_results_api_rule_summaries) | **GET** /tenants/{tenantId}/validations/results-api/jobs/{jobId}/runs/{runId}/rules/summary | Retrieves a list Rule Summaries from the Validation Results API.
[**find_results_api_rules_async**](ValidationResultsAPIApi.md#find_results_api_rules_async) | **GET** /tenants/{tenantId}/validations/results-api/rules | Retrieves a list of Rules from Validation Results API.
[**get_latest_job_run_async**](ValidationResultsAPIApi.md#get_latest_job_run_async) | **GET** /tenants/{tenantId}/validations/results-api/jobs/{jobId}/runs/latest | Retrieves the latest Job Run from the Validation Results API.
[**get_results_api_job_by_id**](ValidationResultsAPIApi.md#get_results_api_job_by_id) | **GET** /tenants/{tenantId}/validations/results-api/jobs/{jobId} | Retrieves a Job by ID from the Validation Results API.
[**get_results_api_job_run_by_id_async**](ValidationResultsAPIApi.md#get_results_api_job_run_by_id_async) | **GET** /tenants/{tenantId}/validations/results-api/jobs/{jobId}/runs/{runId} | Retrieves a Job Run by ID from the Validation Results API.
[**get_results_api_job_run_rule_by_id_async**](ValidationResultsAPIApi.md#get_results_api_job_run_rule_by_id_async) | **GET** /tenants/{tenantId}/validations/results-api/jobs/{jobId}/runs/{runId}/rules/{ruleId} | Retrieves a Job Run Rule by ID from the Validation Results API.
[**get_results_api_rule_by_id_async**](ValidationResultsAPIApi.md#get_results_api_rule_by_id_async) | **GET** /tenants/{tenantId}/validations/results-api/rules/{ruleId} | Retrieves a Rule by ID from the Validation Results API.
[**get_results_api_rule_summary**](ValidationResultsAPIApi.md#get_results_api_rule_summary) | **GET** /tenants/{tenantId}/validations/results-api/jobs/{jobId}/runs/{runId}/rules/{ruleId}/summary | Get Rule Summary by ID from the Validation Results API.


# **find_results_api_job_run_records_async**
> List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRecordsRecordDto] find_results_api_job_run_records_async(tenant_id, job_id, run_id, offset=offset, limit=limit)

Retrieves a list of Job Run Records from the Validation Results API.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_validation_results_api_records_record_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRecordsRecordDto
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
    api_instance = edgraph_platform_client.ValidationResultsAPIApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 
    run_id = 'run_id_example' # str | 
    offset = 0 # int |  (optional) (default to 0)
    limit = 25 # int |  (optional) (default to 25)

    try:
        # Retrieves a list of Job Run Records from the Validation Results API.
        api_response = api_instance.find_results_api_job_run_records_async(tenant_id, job_id, run_id, offset=offset, limit=limit)
        print("The response of ValidationResultsAPIApi->find_results_api_job_run_records_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationResultsAPIApi->find_results_api_job_run_records_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 
 **run_id** | **str**|  | 
 **offset** | **int**|  | [optional] [default to 0]
 **limit** | **int**|  | [optional] [default to 25]

### Return type

[**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRecordsRecordDto]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRecordsRecordDto.md)

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

# **find_results_api_job_run_rule_records_async**
> List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRecordsRecordDto] find_results_api_job_run_rule_records_async(tenant_id, job_id, run_id, rule_id, offset=offset, limit=limit)

Retrieves a list of Job Run Rule Records from the Validation Results API.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_validation_results_api_records_record_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRecordsRecordDto
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
    api_instance = edgraph_platform_client.ValidationResultsAPIApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 
    run_id = 'run_id_example' # str | 
    rule_id = 'rule_id_example' # str | 
    offset = 0 # int |  (optional) (default to 0)
    limit = 25 # int |  (optional) (default to 25)

    try:
        # Retrieves a list of Job Run Rule Records from the Validation Results API.
        api_response = api_instance.find_results_api_job_run_rule_records_async(tenant_id, job_id, run_id, rule_id, offset=offset, limit=limit)
        print("The response of ValidationResultsAPIApi->find_results_api_job_run_rule_records_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationResultsAPIApi->find_results_api_job_run_rule_records_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 
 **run_id** | **str**|  | 
 **rule_id** | **str**|  | 
 **offset** | **int**|  | [optional] [default to 0]
 **limit** | **int**|  | [optional] [default to 25]

### Return type

[**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRecordsRecordDto]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRecordsRecordDto.md)

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

# **find_results_api_job_run_rules_async**
> List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRulesRuleDto] find_results_api_job_run_rules_async(tenant_id, job_id, run_id, offset=offset, limit=limit)

Retrieves a list of Job Run Rules from the Validation Results API.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_validation_results_api_rules_rule_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRulesRuleDto
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
    api_instance = edgraph_platform_client.ValidationResultsAPIApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 
    run_id = 'run_id_example' # str | 
    offset = 0 # int |  (optional) (default to 0)
    limit = 25 # int |  (optional) (default to 25)

    try:
        # Retrieves a list of Job Run Rules from the Validation Results API.
        api_response = api_instance.find_results_api_job_run_rules_async(tenant_id, job_id, run_id, offset=offset, limit=limit)
        print("The response of ValidationResultsAPIApi->find_results_api_job_run_rules_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationResultsAPIApi->find_results_api_job_run_rules_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 
 **run_id** | **str**|  | 
 **offset** | **int**|  | [optional] [default to 0]
 **limit** | **int**|  | [optional] [default to 25]

### Return type

[**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRulesRuleDto]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRulesRuleDto.md)

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

# **find_results_api_job_runs_async**
> List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRunsRunDto] find_results_api_job_runs_async(tenant_id, job_id, offset=offset, limit=limit)

Retrieves a list of Job Runs from the Validation Results API.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_validation_results_api_runs_run_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRunsRunDto
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
    api_instance = edgraph_platform_client.ValidationResultsAPIApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 
    offset = 0 # int |  (optional) (default to 0)
    limit = 25 # int |  (optional) (default to 25)

    try:
        # Retrieves a list of Job Runs from the Validation Results API.
        api_response = api_instance.find_results_api_job_runs_async(tenant_id, job_id, offset=offset, limit=limit)
        print("The response of ValidationResultsAPIApi->find_results_api_job_runs_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationResultsAPIApi->find_results_api_job_runs_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 
 **offset** | **int**|  | [optional] [default to 0]
 **limit** | **int**|  | [optional] [default to 25]

### Return type

[**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRunsRunDto]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRunsRunDto.md)

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

# **find_results_api_jobs_async**
> List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiJobsJobDto] find_results_api_jobs_async(tenant_id, offset=offset, limit=limit)

Retrieves a list of Jobs from the Validation Results API.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_validation_results_api_jobs_job_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiJobsJobDto
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
    api_instance = edgraph_platform_client.ValidationResultsAPIApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    offset = 0 # int |  (optional) (default to 0)
    limit = 25 # int |  (optional) (default to 25)

    try:
        # Retrieves a list of Jobs from the Validation Results API.
        api_response = api_instance.find_results_api_jobs_async(tenant_id, offset=offset, limit=limit)
        print("The response of ValidationResultsAPIApi->find_results_api_jobs_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationResultsAPIApi->find_results_api_jobs_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **offset** | **int**|  | [optional] [default to 0]
 **limit** | **int**|  | [optional] [default to 25]

### Return type

[**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiJobsJobDto]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiJobsJobDto.md)

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

# **find_results_api_rule_summaries**
> List[ValidationsApiResultsV1RuleSummary] find_results_api_rule_summaries(tenant_id, job_id, run_id, offset=offset, limit=limit)

Retrieves a list Rule Summaries from the Validation Results API.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_results_v1_rule_summary import ValidationsApiResultsV1RuleSummary
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
    api_instance = edgraph_platform_client.ValidationResultsAPIApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 
    run_id = 'run_id_example' # str | 
    offset = 0 # int |  (optional) (default to 0)
    limit = 25 # int |  (optional) (default to 25)

    try:
        # Retrieves a list Rule Summaries from the Validation Results API.
        api_response = api_instance.find_results_api_rule_summaries(tenant_id, job_id, run_id, offset=offset, limit=limit)
        print("The response of ValidationResultsAPIApi->find_results_api_rule_summaries:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationResultsAPIApi->find_results_api_rule_summaries: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 
 **run_id** | **str**|  | 
 **offset** | **int**|  | [optional] [default to 0]
 **limit** | **int**|  | [optional] [default to 25]

### Return type

[**List[ValidationsApiResultsV1RuleSummary]**](ValidationsApiResultsV1RuleSummary.md)

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

# **find_results_api_rules_async**
> List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRulesRuleDto] find_results_api_rules_async(tenant_id, offset=offset, limit=limit)

Retrieves a list of Rules from Validation Results API.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_validation_results_api_rules_rule_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRulesRuleDto
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
    api_instance = edgraph_platform_client.ValidationResultsAPIApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    offset = 0 # int |  (optional) (default to 0)
    limit = 25 # int |  (optional) (default to 25)

    try:
        # Retrieves a list of Rules from Validation Results API.
        api_response = api_instance.find_results_api_rules_async(tenant_id, offset=offset, limit=limit)
        print("The response of ValidationResultsAPIApi->find_results_api_rules_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationResultsAPIApi->find_results_api_rules_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **offset** | **int**|  | [optional] [default to 0]
 **limit** | **int**|  | [optional] [default to 25]

### Return type

[**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRulesRuleDto]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRulesRuleDto.md)

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

# **get_latest_job_run_async**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRunsRunDto get_latest_job_run_async(tenant_id, job_id)

Retrieves the latest Job Run from the Validation Results API.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_validation_results_api_runs_run_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRunsRunDto
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
    api_instance = edgraph_platform_client.ValidationResultsAPIApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 

    try:
        # Retrieves the latest Job Run from the Validation Results API.
        api_response = api_instance.get_latest_job_run_async(tenant_id, job_id)
        print("The response of ValidationResultsAPIApi->get_latest_job_run_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationResultsAPIApi->get_latest_job_run_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRunsRunDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRunsRunDto.md)

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

# **get_results_api_job_by_id**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiJobsJobDto get_results_api_job_by_id(tenant_id, job_id)

Retrieves a Job by ID from the Validation Results API.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_validation_results_api_jobs_job_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiJobsJobDto
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
    api_instance = edgraph_platform_client.ValidationResultsAPIApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 

    try:
        # Retrieves a Job by ID from the Validation Results API.
        api_response = api_instance.get_results_api_job_by_id(tenant_id, job_id)
        print("The response of ValidationResultsAPIApi->get_results_api_job_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationResultsAPIApi->get_results_api_job_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiJobsJobDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiJobsJobDto.md)

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

# **get_results_api_job_run_by_id_async**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRunsRunDto get_results_api_job_run_by_id_async(tenant_id, job_id, run_id)

Retrieves a Job Run by ID from the Validation Results API.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_validation_results_api_runs_run_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRunsRunDto
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
    api_instance = edgraph_platform_client.ValidationResultsAPIApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 
    run_id = 'run_id_example' # str | 

    try:
        # Retrieves a Job Run by ID from the Validation Results API.
        api_response = api_instance.get_results_api_job_run_by_id_async(tenant_id, job_id, run_id)
        print("The response of ValidationResultsAPIApi->get_results_api_job_run_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationResultsAPIApi->get_results_api_job_run_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 
 **run_id** | **str**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRunsRunDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRunsRunDto.md)

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

# **get_results_api_job_run_rule_by_id_async**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRulesRuleDto get_results_api_job_run_rule_by_id_async(tenant_id, job_id, run_id, rule_id)

Retrieves a Job Run Rule by ID from the Validation Results API.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_validation_results_api_rules_rule_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRulesRuleDto
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
    api_instance = edgraph_platform_client.ValidationResultsAPIApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 
    run_id = 'run_id_example' # str | 
    rule_id = 'rule_id_example' # str | 

    try:
        # Retrieves a Job Run Rule by ID from the Validation Results API.
        api_response = api_instance.get_results_api_job_run_rule_by_id_async(tenant_id, job_id, run_id, rule_id)
        print("The response of ValidationResultsAPIApi->get_results_api_job_run_rule_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationResultsAPIApi->get_results_api_job_run_rule_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 
 **run_id** | **str**|  | 
 **rule_id** | **str**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRulesRuleDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRulesRuleDto.md)

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

# **get_results_api_rule_by_id_async**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRulesRuleDto get_results_api_rule_by_id_async(tenant_id, rule_id)

Retrieves a Rule by ID from the Validation Results API.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_validation_results_api_rules_rule_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRulesRuleDto
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
    api_instance = edgraph_platform_client.ValidationResultsAPIApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    rule_id = 'rule_id_example' # str | 

    try:
        # Retrieves a Rule by ID from the Validation Results API.
        api_response = api_instance.get_results_api_rule_by_id_async(tenant_id, rule_id)
        print("The response of ValidationResultsAPIApi->get_results_api_rule_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationResultsAPIApi->get_results_api_rule_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **rule_id** | **str**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRulesRuleDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiRulesRuleDto.md)

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

# **get_results_api_rule_summary**
> ValidationsApiResultsV1RuleSummary get_results_api_rule_summary(tenant_id, job_id, run_id, rule_id)

Get Rule Summary by ID from the Validation Results API.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_results_v1_rule_summary import ValidationsApiResultsV1RuleSummary
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
    api_instance = edgraph_platform_client.ValidationResultsAPIApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    job_id = 'job_id_example' # str | 
    run_id = 'run_id_example' # str | 
    rule_id = 'rule_id_example' # str | 

    try:
        # Get Rule Summary by ID from the Validation Results API.
        api_response = api_instance.get_results_api_rule_summary(tenant_id, job_id, run_id, rule_id)
        print("The response of ValidationResultsAPIApi->get_results_api_rule_summary:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationResultsAPIApi->get_results_api_rule_summary: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **job_id** | **str**|  | 
 **run_id** | **str**|  | 
 **rule_id** | **str**|  | 

### Return type

[**ValidationsApiResultsV1RuleSummary**](ValidationsApiResultsV1RuleSummary.md)

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

