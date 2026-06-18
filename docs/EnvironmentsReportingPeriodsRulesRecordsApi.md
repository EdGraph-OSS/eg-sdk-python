# edgraph_platform_client.EnvironmentsReportingPeriodsRulesRecordsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_state_reporting_period_rules**](EnvironmentsReportingPeriodsRulesRecordsApi.md#delete_state_reporting_period_rules) | **DELETE** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/rules | Deletes the Rules of a Reporting Period.
[**search_state_reporting_period_records**](EnvironmentsReportingPeriodsRulesRecordsApi.md#search_state_reporting_period_records) | **GET** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/records | Retrieves the Invalid Records of all the Rules within a Reporting Period.
[**search_state_reporting_period_rule_records**](EnvironmentsReportingPeriodsRulesRecordsApi.md#search_state_reporting_period_rule_records) | **GET** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/rules/{ruleId}/records | Retrieves the Invalid Records of a Rule.
[**set_state_reporting_period_rule_record_post_flag**](EnvironmentsReportingPeriodsRulesRecordsApi.md#set_state_reporting_period_rule_record_post_flag) | **PUT** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/rules/{ruleId}/records/{recordId}/excludefrompost | Toggles the \&quot;ExcludeFromPost\&quot; flag of a Rule&#39;s Invalid Record.
[**set_state_reporting_period_rule_record_post_flag_bulk**](EnvironmentsReportingPeriodsRulesRecordsApi.md#set_state_reporting_period_rule_record_post_flag_bulk) | **PUT** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/rules/{ruleId}/records/excludefrompost | Toggles the \&quot;ExcludeFromPost\&quot; flag of a Rule&#39;s Invalid Records in bulk.


# **delete_state_reporting_period_rules**
> EdGraphServicesStateReportingV1ReportingPeriodRulesDeletedResponse delete_state_reporting_period_rules(tenant_id, environment_id, reporting_period_id)

Deletes the Rules of a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_rules_deleted_response import EdGraphServicesStateReportingV1ReportingPeriodRulesDeletedResponse
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsRulesRecordsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    reporting_period_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Deletes the Rules of a Reporting Period.
        api_response = await api_instance.delete_state_reporting_period_rules(tenant_id, environment_id, reporting_period_id)
        print("The response of EnvironmentsReportingPeriodsRulesRecordsApi->delete_state_reporting_period_rules:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsRulesRecordsApi->delete_state_reporting_period_rules: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **reporting_period_id** | **UUID**|  | 

### Return type

[**EdGraphServicesStateReportingV1ReportingPeriodRulesDeletedResponse**](EdGraphServicesStateReportingV1ReportingPeriodRulesDeletedResponse.md)

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

# **search_state_reporting_period_records**
> EdGraphServicesStateReportingV1PaginatedRecords search_state_reporting_period_records(tenant_id, environment_id, reporting_period_id, page_index=page_index, page_size=page_size, exclude_from_post=exclude_from_post)

Retrieves the Invalid Records of all the Rules within a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_paginated_records import EdGraphServicesStateReportingV1PaginatedRecords
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsRulesRecordsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    reporting_period_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_index = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    exclude_from_post = True # bool |  (optional)

    try:
        # Retrieves the Invalid Records of all the Rules within a Reporting Period.
        api_response = await api_instance.search_state_reporting_period_records(tenant_id, environment_id, reporting_period_id, page_index=page_index, page_size=page_size, exclude_from_post=exclude_from_post)
        print("The response of EnvironmentsReportingPeriodsRulesRecordsApi->search_state_reporting_period_records:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsRulesRecordsApi->search_state_reporting_period_records: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **reporting_period_id** | **UUID**|  | 
 **page_index** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **exclude_from_post** | **bool**|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1PaginatedRecords**](EdGraphServicesStateReportingV1PaginatedRecords.md)

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

# **search_state_reporting_period_rule_records**
> EdGraphServicesStateReportingV1PaginatedRuleRecords search_state_reporting_period_rule_records(tenant_id, environment_id, reporting_period_id, rule_id, page_index=page_index, page_size=page_size)

Retrieves the Invalid Records of a Rule.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_paginated_rule_records import EdGraphServicesStateReportingV1PaginatedRuleRecords
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsRulesRecordsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    reporting_period_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    rule_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_index = 56 # int |  (optional)
    page_size = 56 # int |  (optional)

    try:
        # Retrieves the Invalid Records of a Rule.
        api_response = await api_instance.search_state_reporting_period_rule_records(tenant_id, environment_id, reporting_period_id, rule_id, page_index=page_index, page_size=page_size)
        print("The response of EnvironmentsReportingPeriodsRulesRecordsApi->search_state_reporting_period_rule_records:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsRulesRecordsApi->search_state_reporting_period_rule_records: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **reporting_period_id** | **UUID**|  | 
 **rule_id** | **UUID**|  | 
 **page_index** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1PaginatedRuleRecords**](EdGraphServicesStateReportingV1PaginatedRuleRecords.md)

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

# **set_state_reporting_period_rule_record_post_flag**
> EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse set_state_reporting_period_rule_record_post_flag(tenant_id, environment_id, reporting_period_id, rule_id, record_id, ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_request=ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_request)

Toggles the \"ExcludeFromPost\" flag of a Rule's Invalid Record.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_created_response import EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_request import EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagRequest
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsRulesRecordsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    reporting_period_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    rule_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    record_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_request = edgraph_platform_client.EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagRequest() # EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagRequest |  (optional)

    try:
        # Toggles the \"ExcludeFromPost\" flag of a Rule's Invalid Record.
        api_response = await api_instance.set_state_reporting_period_rule_record_post_flag(tenant_id, environment_id, reporting_period_id, rule_id, record_id, ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_request=ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_request)
        print("The response of EnvironmentsReportingPeriodsRulesRecordsApi->set_state_reporting_period_rule_record_post_flag:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsRulesRecordsApi->set_state_reporting_period_rule_record_post_flag: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **reporting_period_id** | **UUID**|  | 
 **rule_id** | **UUID**|  | 
 **record_id** | **UUID**|  | 
 **ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_request** | [**EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagRequest**](EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagRequest.md)|  | [optional] 

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

# **set_state_reporting_period_rule_record_post_flag_bulk**
> EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse set_state_reporting_period_rule_record_post_flag_bulk(tenant_id, environment_id, reporting_period_id, rule_id, ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_bulk_request=ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_bulk_request)

Toggles the \"ExcludeFromPost\" flag of a Rule's Invalid Records in bulk.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_created_response import EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_bulk_request import EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagBulkRequest
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsRulesRecordsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    reporting_period_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    rule_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_bulk_request = edgraph_platform_client.EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagBulkRequest() # EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagBulkRequest |  (optional)

    try:
        # Toggles the \"ExcludeFromPost\" flag of a Rule's Invalid Records in bulk.
        api_response = await api_instance.set_state_reporting_period_rule_record_post_flag_bulk(tenant_id, environment_id, reporting_period_id, rule_id, ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_bulk_request=ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_bulk_request)
        print("The response of EnvironmentsReportingPeriodsRulesRecordsApi->set_state_reporting_period_rule_record_post_flag_bulk:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsRulesRecordsApi->set_state_reporting_period_rule_record_post_flag_bulk: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **reporting_period_id** | **UUID**|  | 
 **rule_id** | **UUID**|  | 
 **ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_bulk_request** | [**EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagBulkRequest**](EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagBulkRequest.md)|  | [optional] 

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

