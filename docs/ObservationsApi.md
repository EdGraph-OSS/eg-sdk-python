# edgraph_platform_client.ObservationsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_observation**](ObservationsApi.md#create_observation) | **POST** /tenants/{tenantId}/observations | Creates a new Observation for a given tenant
[**create_observation_submission**](ObservationsApi.md#create_observation_submission) | **POST** /tenants/{tenantId}/observations/{observationId}/available-forms/{formId}/submit | Creates a submission for an available form referencing an existing observation
[**delete_observation**](ObservationsApi.md#delete_observation) | **DELETE** /tenants/{tenantId}/observations/{observationId} | Deletes an Observation for a given tenant
[**get_dashboard**](ObservationsApi.md#get_dashboard) | **GET** /tenants/{tenantId}/observations/dashboards/{dashboardId} | Get Observation Dashboard
[**get_dashboard_preferences**](ObservationsApi.md#get_dashboard_preferences) | **GET** /tenants/{tenantId}/observations/dashboards/{dashboardId}/preferences | Save user preferences for a given Dashboard
[**get_evaluee_sections**](ObservationsApi.md#get_evaluee_sections) | **GET** /tenants/{tenantId}/observations/evaluees/{evalueeId}/sections | Gets the Sections of an evaluee.
[**get_form_questions**](ObservationsApi.md#get_form_questions) | **GET** /tenants/{tenantId}/observations/available-forms/{formId}/sections/{sectionId}/questions | Search Questions
[**get_form_sections**](ObservationsApi.md#get_form_sections) | **GET** /tenants/{tenantId}/observations/available-forms/{formId}/sections | Search Observation Form Sections
[**get_observation_by_id**](ObservationsApi.md#get_observation_by_id) | **GET** /tenants/{tenantId}/observations/{observationId} | Get an Observation for a given tenant
[**get_observation_draft**](ObservationsApi.md#get_observation_draft) | **GET** /tenants/{tenantId}/observations/{observationId}/available-forms/{formId}/draft | Get an observation form&#39;s draft
[**get_observation_submission**](ObservationsApi.md#get_observation_submission) | **GET** /tenants/{tenantId}/observations/{observationId}/available-forms/{formId}/submission | Gets a submission for a specific observation
[**get_paginated_available_campuses**](ObservationsApi.md#get_paginated_available_campuses) | **GET** /tenants/{tenantId}/observations/campuses | Get Available Campuses
[**get_paginated_available_forms**](ObservationsApi.md#get_paginated_available_forms) | **GET** /tenants/{tenantId}/observations/available-forms | Get Paginated Available Forms
[**get_paginated_campus_sections**](ObservationsApi.md#get_paginated_campus_sections) | **GET** /tenants/{tenantId}/observations/campuses/{campusId}/sections | Retrieves a list of Sections for a given available campus.
[**get_paginated_evaluees**](ObservationsApi.md#get_paginated_evaluees) | **GET** /tenants/{tenantId}/observations/evaluees | Get paginated evaluees
[**get_paginated_observations**](ObservationsApi.md#get_paginated_observations) | **GET** /tenants/{tenantId}/observations | Get Paginated Observations for a given tenant
[**get_submitted_observations_count**](ObservationsApi.md#get_submitted_observations_count) | **GET** /tenants/{tenantId}/submittedobservations | Get submitted Observations count
[**save_dashboard_preferences**](ObservationsApi.md#save_dashboard_preferences) | **POST** /tenants/{tenantId}/observations/dashboards/{dashboardId}/preferences | Save user preferences for a given Dashboard
[**update_observation**](ObservationsApi.md#update_observation) | **PUT** /tenants/{tenantId}/observations/{observationId} | Update an Observation for a given tenant
[**upsert_observation_draft**](ObservationsApi.md#upsert_observation_draft) | **POST** /tenants/{tenantId}/observations/{observationId}/available-forms/{formId}/draft | Creates a draft for an observation forms
[**verify_dashboard_access**](ObservationsApi.md#verify_dashboard_access) | **POST** /tenants/{tenantId}/observations/dashboards/access | Verify user access to dashboards


# **create_observation**
> EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationResponse create_observation(tenant_id, ed_graph_http_aggregators_tenant_api_services_observations_create_observation_request=ed_graph_http_aggregators_tenant_api_services_observations_create_observation_request)

Creates a new Observation for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_create_observation_request import EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationRequest
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_create_observation_response import EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_services_observations_create_observation_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationRequest() # EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationRequest |  (optional)

    try:
        # Creates a new Observation for a given tenant
        api_response = api_instance.create_observation(tenant_id, ed_graph_http_aggregators_tenant_api_services_observations_create_observation_request=ed_graph_http_aggregators_tenant_api_services_observations_create_observation_request)
        print("The response of ObservationsApi->create_observation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->create_observation: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_services_observations_create_observation_request** | [**EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationRequest**](EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationRequest.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationResponse.md)

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

# **create_observation_submission**
> EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationSubmissionResponse create_observation_submission(tenant_id, form_id, observation_id, ed_graph_http_aggregators_tenant_api_services_observations_create_observation_submission_request=ed_graph_http_aggregators_tenant_api_services_observations_create_observation_submission_request)

Creates a submission for an available form referencing an existing observation

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_create_observation_submission_request import EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationSubmissionRequest
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_create_observation_submission_response import EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationSubmissionResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    form_id = 'form_id_example' # str | 
    observation_id = 'observation_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_services_observations_create_observation_submission_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationSubmissionRequest() # EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationSubmissionRequest |  (optional)

    try:
        # Creates a submission for an available form referencing an existing observation
        api_response = api_instance.create_observation_submission(tenant_id, form_id, observation_id, ed_graph_http_aggregators_tenant_api_services_observations_create_observation_submission_request=ed_graph_http_aggregators_tenant_api_services_observations_create_observation_submission_request)
        print("The response of ObservationsApi->create_observation_submission:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->create_observation_submission: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **form_id** | **str**|  | 
 **observation_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_services_observations_create_observation_submission_request** | [**EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationSubmissionRequest**](EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationSubmissionRequest.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationSubmissionResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationSubmissionResponse.md)

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

# **delete_observation**
> EdGraphHttpAggregatorsTenantApiServicesObservationsDeleteObservationResponse delete_observation(tenant_id, observation_id)

Deletes an Observation for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_delete_observation_response import EdGraphHttpAggregatorsTenantApiServicesObservationsDeleteObservationResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    observation_id = 'observation_id_example' # str | 

    try:
        # Deletes an Observation for a given tenant
        api_response = api_instance.delete_observation(tenant_id, observation_id)
        print("The response of ObservationsApi->delete_observation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->delete_observation: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **observation_id** | **str**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsDeleteObservationResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsDeleteObservationResponse.md)

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

# **get_dashboard**
> AnalyticsApiReportsV1ReportResponse get_dashboard(tenant_id, dashboard_id, persona_identifier=persona_identifier)

Get Observation Dashboard

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_reports_v1_report_response import AnalyticsApiReportsV1ReportResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    dashboard_id = 'dashboard_id_example' # str | 
    persona_identifier = 'persona_identifier_example' # str |  (optional)

    try:
        # Get Observation Dashboard
        api_response = api_instance.get_dashboard(tenant_id, dashboard_id, persona_identifier=persona_identifier)
        print("The response of ObservationsApi->get_dashboard:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_dashboard: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **dashboard_id** | **str**|  | 
 **persona_identifier** | **str**|  | [optional] 

### Return type

[**AnalyticsApiReportsV1ReportResponse**](AnalyticsApiReportsV1ReportResponse.md)

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

# **get_dashboard_preferences**
> AnalyticsApiReportsV1ReportPreferencesResponse get_dashboard_preferences(tenant_id, dashboard_id)

Save user preferences for a given Dashboard

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_reports_v1_report_preferences_response import AnalyticsApiReportsV1ReportPreferencesResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    dashboard_id = 'dashboard_id_example' # str | 

    try:
        # Save user preferences for a given Dashboard
        api_response = api_instance.get_dashboard_preferences(tenant_id, dashboard_id)
        print("The response of ObservationsApi->get_dashboard_preferences:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_dashboard_preferences: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **dashboard_id** | **str**|  | 

### Return type

[**AnalyticsApiReportsV1ReportPreferencesResponse**](AnalyticsApiReportsV1ReportPreferencesResponse.md)

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

# **get_evaluee_sections**
> IdentityApiUserV1SectionResponseGetPaginatedItemsResponse get_evaluee_sections(tenant_id, evaluee_id, page_index=page_index, page_size=page_size, order_by=order_by, filter_by=filter_by)

Gets the Sections of an evaluee.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_user_v1_section_response_get_paginated_items_response import IdentityApiUserV1SectionResponseGetPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    evaluee_id = 'evaluee_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter_by = '' # str |  (optional) (default to '')

    try:
        # Gets the Sections of an evaluee.
        api_response = api_instance.get_evaluee_sections(tenant_id, evaluee_id, page_index=page_index, page_size=page_size, order_by=order_by, filter_by=filter_by)
        print("The response of ObservationsApi->get_evaluee_sections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_evaluee_sections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **evaluee_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter_by** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**IdentityApiUserV1SectionResponseGetPaginatedItemsResponse**](IdentityApiUserV1SectionResponseGetPaginatedItemsResponse.md)

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

# **get_form_questions**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesFormsQuestionResponseDtoPaginatedItemsViewModel get_form_questions(tenant_id, form_id, section_id, page_index=page_index, page_size=page_size)

Search Questions

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_forms_question_response_dto_paginated_items_view_model import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesFormsQuestionResponseDtoPaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    form_id = 'form_id_example' # str | 
    section_id = 'section_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)

    try:
        # Search Questions
        api_response = api_instance.get_form_questions(tenant_id, form_id, section_id, page_index=page_index, page_size=page_size)
        print("The response of ObservationsApi->get_form_questions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_form_questions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **form_id** | **str**|  | 
 **section_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesFormsQuestionResponseDtoPaginatedItemsViewModel**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesFormsQuestionResponseDtoPaginatedItemsViewModel.md)

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

# **get_form_sections**
> EdGraphHttpAggregatorsTenantApiServicesObservationsFormSectionResponsePaginatedItemsViewModel get_form_sections(tenant_id, form_id, page_index=page_index, page_size=page_size)

Search Observation Form Sections

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_form_section_response_paginated_items_view_model import EdGraphHttpAggregatorsTenantApiServicesObservationsFormSectionResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    form_id = 'form_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)

    try:
        # Search Observation Form Sections
        api_response = api_instance.get_form_sections(tenant_id, form_id, page_index=page_index, page_size=page_size)
        print("The response of ObservationsApi->get_form_sections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_form_sections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **form_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsFormSectionResponsePaginatedItemsViewModel**](EdGraphHttpAggregatorsTenantApiServicesObservationsFormSectionResponsePaginatedItemsViewModel.md)

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

# **get_observation_by_id**
> EdGraphHttpAggregatorsTenantApiServicesObservationsObservationProfileResponse get_observation_by_id(tenant_id, observation_id)

Get an Observation for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_observation_profile_response import EdGraphHttpAggregatorsTenantApiServicesObservationsObservationProfileResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    observation_id = 'observation_id_example' # str | 

    try:
        # Get an Observation for a given tenant
        api_response = api_instance.get_observation_by_id(tenant_id, observation_id)
        print("The response of ObservationsApi->get_observation_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_observation_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **observation_id** | **str**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsObservationProfileResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsObservationProfileResponse.md)

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

# **get_observation_draft**
> EdGraphHttpAggregatorsTenantApiServicesObservationsObservationDraftResponse get_observation_draft(tenant_id, observation_id, form_id)

Get an observation form's draft

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_observation_draft_response import EdGraphHttpAggregatorsTenantApiServicesObservationsObservationDraftResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    observation_id = 'observation_id_example' # str | 
    form_id = 'form_id_example' # str | 

    try:
        # Get an observation form's draft
        api_response = api_instance.get_observation_draft(tenant_id, observation_id, form_id)
        print("The response of ObservationsApi->get_observation_draft:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_observation_draft: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **observation_id** | **str**|  | 
 **form_id** | **str**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsObservationDraftResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsObservationDraftResponse.md)

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

# **get_observation_submission**
> EdGraphHttpAggregatorsTenantApiServicesObservationsObservationSubmissionResponse get_observation_submission(tenant_id, observation_id, form_id)

Gets a submission for a specific observation

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_observation_submission_response import EdGraphHttpAggregatorsTenantApiServicesObservationsObservationSubmissionResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    observation_id = 'observation_id_example' # str | 
    form_id = 'form_id_example' # str | 

    try:
        # Gets a submission for a specific observation
        api_response = api_instance.get_observation_submission(tenant_id, observation_id, form_id)
        print("The response of ObservationsApi->get_observation_submission:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_observation_submission: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **observation_id** | **str**|  | 
 **form_id** | **str**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsObservationSubmissionResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsObservationSubmissionResponse.md)

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

# **get_paginated_available_campuses**
> EdGraphHttpAggregatorsTenantApiServicesObservationsCampusResponseGetPaginatedItemsResponse get_paginated_available_campuses(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, name_of_institution=name_of_institution)

Get Available Campuses

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_campus_response_get_paginated_items_response import EdGraphHttpAggregatorsTenantApiServicesObservationsCampusResponseGetPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    name_of_institution = '' # str |  (optional) (default to '')

    try:
        # Get Available Campuses
        api_response = api_instance.get_paginated_available_campuses(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, name_of_institution=name_of_institution)
        print("The response of ObservationsApi->get_paginated_available_campuses:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_paginated_available_campuses: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **name_of_institution** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsCampusResponseGetPaginatedItemsResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsCampusResponseGetPaginatedItemsResponse.md)

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

# **get_paginated_available_forms**
> EdGraphHttpAggregatorsTenantApiServicesObservationsFormResponseGetPaginatedItemsResponse get_paginated_available_forms(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)

Get Paginated Available Forms

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_form_response_get_paginated_items_response import EdGraphHttpAggregatorsTenantApiServicesObservationsFormResponseGetPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Get Paginated Available Forms
        api_response = api_instance.get_paginated_available_forms(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)
        print("The response of ObservationsApi->get_paginated_available_forms:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_paginated_available_forms: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsFormResponseGetPaginatedItemsResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsFormResponseGetPaginatedItemsResponse.md)

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

# **get_paginated_campus_sections**
> TenantApiSectionsV1SectionListResponseGetPaginatedItemsResponse get_paginated_campus_sections(tenant_id, campus_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)

Retrieves a list of Sections for a given available campus.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_sections_v1_section_list_response_get_paginated_items_response import TenantApiSectionsV1SectionListResponseGetPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    campus_id = 'campus_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of Sections for a given available campus.
        api_response = api_instance.get_paginated_campus_sections(tenant_id, campus_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)
        print("The response of ObservationsApi->get_paginated_campus_sections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_paginated_campus_sections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **campus_id** | **str**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**TenantApiSectionsV1SectionListResponseGetPaginatedItemsResponse**](TenantApiSectionsV1SectionListResponseGetPaginatedItemsResponse.md)

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

# **get_paginated_evaluees**
> EdGraphHttpAggregatorsTenantApiServicesObservationsEvalueeResponseGetPaginatedItemsResponse get_paginated_evaluees(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, campus=campus, evaluee_id=evaluee_id, first_name=first_name, last_name=last_name)

Get paginated evaluees

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_evaluee_response_get_paginated_items_response import EdGraphHttpAggregatorsTenantApiServicesObservationsEvalueeResponseGetPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    campus = '' # str |  (optional) (default to '')
    evaluee_id = '' # str |  (optional) (default to '')
    first_name = '' # str |  (optional) (default to '')
    last_name = '' # str |  (optional) (default to '')

    try:
        # Get paginated evaluees
        api_response = api_instance.get_paginated_evaluees(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, campus=campus, evaluee_id=evaluee_id, first_name=first_name, last_name=last_name)
        print("The response of ObservationsApi->get_paginated_evaluees:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_paginated_evaluees: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **campus** | **str**|  | [optional] [default to &#39;&#39;]
 **evaluee_id** | **str**|  | [optional] [default to &#39;&#39;]
 **first_name** | **str**|  | [optional] [default to &#39;&#39;]
 **last_name** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsEvalueeResponseGetPaginatedItemsResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsEvalueeResponseGetPaginatedItemsResponse.md)

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

# **get_paginated_observations**
> EdGraphHttpAggregatorsTenantApiServicesObservationsObservationProfileResponsePaginatedItemsViewModel get_paginated_observations(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, campus=campus, evaluee_name=evaluee_name, evaluee_id=evaluee_id, form_id=form_id, status=status, var_from=var_from, to=to)

Get Paginated Observations for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_observation_profile_response_paginated_items_view_model import EdGraphHttpAggregatorsTenantApiServicesObservationsObservationProfileResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    campus = '' # str |  (optional) (default to '')
    evaluee_name = '' # str |  (optional) (default to '')
    evaluee_id = '' # str |  (optional) (default to '')
    form_id = '' # str |  (optional) (default to '')
    status = '' # str |  (optional) (default to '')
    var_from = '' # str |  (optional) (default to '')
    to = '' # str |  (optional) (default to '')

    try:
        # Get Paginated Observations for a given tenant
        api_response = api_instance.get_paginated_observations(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, campus=campus, evaluee_name=evaluee_name, evaluee_id=evaluee_id, form_id=form_id, status=status, var_from=var_from, to=to)
        print("The response of ObservationsApi->get_paginated_observations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_paginated_observations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **campus** | **str**|  | [optional] [default to &#39;&#39;]
 **evaluee_name** | **str**|  | [optional] [default to &#39;&#39;]
 **evaluee_id** | **str**|  | [optional] [default to &#39;&#39;]
 **form_id** | **str**|  | [optional] [default to &#39;&#39;]
 **status** | **str**|  | [optional] [default to &#39;&#39;]
 **var_from** | **str**|  | [optional] [default to &#39;&#39;]
 **to** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsObservationProfileResponsePaginatedItemsViewModel**](EdGraphHttpAggregatorsTenantApiServicesObservationsObservationProfileResponsePaginatedItemsViewModel.md)

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

# **get_submitted_observations_count**
> EdGraphHttpAggregatorsTenantApiServicesObservationsGetSubmittedObservationsCountResponse get_submitted_observations_count(tenant_id, evaluee_id=evaluee_id, campus=campus)

Get submitted Observations count

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_get_submitted_observations_count_response import EdGraphHttpAggregatorsTenantApiServicesObservationsGetSubmittedObservationsCountResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    evaluee_id = 'evaluee_id_example' # str |  (optional)
    campus = 'campus_example' # str |  (optional)

    try:
        # Get submitted Observations count
        api_response = api_instance.get_submitted_observations_count(tenant_id, evaluee_id=evaluee_id, campus=campus)
        print("The response of ObservationsApi->get_submitted_observations_count:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_submitted_observations_count: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **evaluee_id** | **str**|  | [optional] 
 **campus** | **str**|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsGetSubmittedObservationsCountResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsGetSubmittedObservationsCountResponse.md)

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

# **save_dashboard_preferences**
> AnalyticsApiReportsV1ReportPreferencesSavedResponse save_dashboard_preferences(tenant_id, dashboard_id, ed_graph_http_aggregators_tenant_api_services_observations_upsert_dashboard_preferences_request=ed_graph_http_aggregators_tenant_api_services_observations_upsert_dashboard_preferences_request)

Save user preferences for a given Dashboard

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_reports_v1_report_preferences_saved_response import AnalyticsApiReportsV1ReportPreferencesSavedResponse
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_upsert_dashboard_preferences_request import EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertDashboardPreferencesRequest
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    dashboard_id = 'dashboard_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_services_observations_upsert_dashboard_preferences_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertDashboardPreferencesRequest() # EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertDashboardPreferencesRequest |  (optional)

    try:
        # Save user preferences for a given Dashboard
        api_response = api_instance.save_dashboard_preferences(tenant_id, dashboard_id, ed_graph_http_aggregators_tenant_api_services_observations_upsert_dashboard_preferences_request=ed_graph_http_aggregators_tenant_api_services_observations_upsert_dashboard_preferences_request)
        print("The response of ObservationsApi->save_dashboard_preferences:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->save_dashboard_preferences: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **dashboard_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_services_observations_upsert_dashboard_preferences_request** | [**EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertDashboardPreferencesRequest**](EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertDashboardPreferencesRequest.md)|  | [optional] 

### Return type

[**AnalyticsApiReportsV1ReportPreferencesSavedResponse**](AnalyticsApiReportsV1ReportPreferencesSavedResponse.md)

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

# **update_observation**
> EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationResponse update_observation(tenant_id, observation_id, ed_graph_http_aggregators_tenant_api_services_observations_update_observation_request=ed_graph_http_aggregators_tenant_api_services_observations_update_observation_request)

Update an Observation for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_update_observation_request import EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationRequest
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_update_observation_response import EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    observation_id = 'observation_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_services_observations_update_observation_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationRequest() # EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationRequest |  (optional)

    try:
        # Update an Observation for a given tenant
        api_response = api_instance.update_observation(tenant_id, observation_id, ed_graph_http_aggregators_tenant_api_services_observations_update_observation_request=ed_graph_http_aggregators_tenant_api_services_observations_update_observation_request)
        print("The response of ObservationsApi->update_observation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->update_observation: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **observation_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_services_observations_update_observation_request** | [**EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationRequest**](EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationRequest.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationResponse.md)

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

# **upsert_observation_draft**
> EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertObservationDraftResponse upsert_observation_draft(tenant_id, observation_id, form_id, ed_graph_http_aggregators_tenant_api_services_observations_upsert_observation_draft_request=ed_graph_http_aggregators_tenant_api_services_observations_upsert_observation_draft_request)

Creates a draft for an observation forms

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_upsert_observation_draft_request import EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertObservationDraftRequest
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_upsert_observation_draft_response import EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertObservationDraftResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    observation_id = 'observation_id_example' # str | 
    form_id = 'form_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_services_observations_upsert_observation_draft_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertObservationDraftRequest() # EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertObservationDraftRequest |  (optional)

    try:
        # Creates a draft for an observation forms
        api_response = api_instance.upsert_observation_draft(tenant_id, observation_id, form_id, ed_graph_http_aggregators_tenant_api_services_observations_upsert_observation_draft_request=ed_graph_http_aggregators_tenant_api_services_observations_upsert_observation_draft_request)
        print("The response of ObservationsApi->upsert_observation_draft:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->upsert_observation_draft: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **observation_id** | **str**|  | 
 **form_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_services_observations_upsert_observation_draft_request** | [**EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertObservationDraftRequest**](EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertObservationDraftRequest.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertObservationDraftResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertObservationDraftResponse.md)

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

# **verify_dashboard_access**
> EdGraphHttpAggregatorsTenantApiServicesObservationsUseCasesCommandsDashboardAccessResponse verify_dashboard_access(tenant_id, ed_graph_http_aggregators_tenant_api_services_observations_use_cases_commands_dashboard_access_request=ed_graph_http_aggregators_tenant_api_services_observations_use_cases_commands_dashboard_access_request)

Verify user access to dashboards

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_use_cases_commands_dashboard_access_request import EdGraphHttpAggregatorsTenantApiServicesObservationsUseCasesCommandsDashboardAccessRequest
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_use_cases_commands_dashboard_access_response import EdGraphHttpAggregatorsTenantApiServicesObservationsUseCasesCommandsDashboardAccessResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_services_observations_use_cases_commands_dashboard_access_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesObservationsUseCasesCommandsDashboardAccessRequest() # EdGraphHttpAggregatorsTenantApiServicesObservationsUseCasesCommandsDashboardAccessRequest |  (optional)

    try:
        # Verify user access to dashboards
        api_response = api_instance.verify_dashboard_access(tenant_id, ed_graph_http_aggregators_tenant_api_services_observations_use_cases_commands_dashboard_access_request=ed_graph_http_aggregators_tenant_api_services_observations_use_cases_commands_dashboard_access_request)
        print("The response of ObservationsApi->verify_dashboard_access:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->verify_dashboard_access: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_services_observations_use_cases_commands_dashboard_access_request** | [**EdGraphHttpAggregatorsTenantApiServicesObservationsUseCasesCommandsDashboardAccessRequest**](EdGraphHttpAggregatorsTenantApiServicesObservationsUseCasesCommandsDashboardAccessRequest.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsUseCasesCommandsDashboardAccessResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsUseCasesCommandsDashboardAccessResponse.md)

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

