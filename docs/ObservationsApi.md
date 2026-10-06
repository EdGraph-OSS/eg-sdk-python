# edgraph_platform_client.ObservationsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_observation**](ObservationsApi.md#create_observation) | **POST** /tenants/{tenantId}/observations | Creates a new Observation for a given tenant
[**create_observation_submission**](ObservationsApi.md#create_observation_submission) | **POST** /tenants/{tenantId}/observations/{observationId}/available-forms/{formId}/submit | Creates a submission for an available form referencing an existing observation
[**delete_observation**](ObservationsApi.md#delete_observation) | **DELETE** /tenants/{tenantId}/observations/{observationId} | Deletes an Observation for a given tenant
[**execute_user_sync_job**](ObservationsApi.md#execute_user_sync_job) | **POST** /tenants/{tenantId}/observations/usersync/execute | Executes the User Sync job for a given tenant
[**get_academic_subjects_count**](ObservationsApi.md#get_academic_subjects_count) | **GET** /tenants/{tenantId}/observations/academicsubjectscount | Gets the total count of academic subjects for a given tenant
[**get_available_campuses_total_evaluees**](ObservationsApi.md#get_available_campuses_total_evaluees) | **GET** /tenants/{tenantId}/observations/total-evaluees | Get the total number of evaluees across all available campuses
[**get_courses_count**](ObservationsApi.md#get_courses_count) | **GET** /tenants/{tenantId}/observations/coursescount | Gets the total count of courses for a given tenant
[**get_dashboard**](ObservationsApi.md#get_dashboard) | **GET** /tenants/{tenantId}/observations/dashboards/{dashboardId} | Get Observation Dashboard
[**get_dashboard_preferences**](ObservationsApi.md#get_dashboard_preferences) | **GET** /tenants/{tenantId}/observations/dashboards/{dashboardId}/preferences | Save user preferences for a given Dashboard
[**get_default_ed_fi_instance**](ObservationsApi.md#get_default_ed_fi_instance) | **GET** /tenants/{tenantId}/observations/defaultinstance | Gets the default Ed-Fi instance for a given tenant
[**get_education_organizations_count**](ObservationsApi.md#get_education_organizations_count) | **GET** /tenants/{tenantId}/observations/educationorganizationscount | Gets the total count of education organizations for a given tenant, filtered by discriminator
[**get_evaluee_sections**](ObservationsApi.md#get_evaluee_sections) | **GET** /tenants/{tenantId}/observations/evaluees/{evalueeId}/sections | Gets the Sections of an evaluee.
[**get_form_questions**](ObservationsApi.md#get_form_questions) | **GET** /tenants/{tenantId}/observations/available-forms/{formId}/sections/{sectionId}/questions | Search Questions
[**get_form_sections**](ObservationsApi.md#get_form_sections) | **GET** /tenants/{tenantId}/observations/available-forms/{formId}/sections | Search Observation Form Sections
[**get_grade_levels_count**](ObservationsApi.md#get_grade_levels_count) | **GET** /tenants/{tenantId}/observations/gradelevelscount | Gets the total count of grade levels for a given tenant
[**get_observation_by_id**](ObservationsApi.md#get_observation_by_id) | **GET** /tenants/{tenantId}/observations/{observationId} | Get an Observation for a given tenant
[**get_observation_draft**](ObservationsApi.md#get_observation_draft) | **GET** /tenants/{tenantId}/observations/{observationId}/available-forms/{formId}/draft | Get an observation form&#39;s draft
[**get_observation_submission**](ObservationsApi.md#get_observation_submission) | **GET** /tenants/{tenantId}/observations/{observationId}/available-forms/{formId}/submission | Gets a submission for a specific observation
[**get_onboarding**](ObservationsApi.md#get_onboarding) | **GET** /tenants/{tenantId}/observations/onboarding | Gets the Instructional Insights onboarding progress for a given tenant
[**get_paginated_available_campuses**](ObservationsApi.md#get_paginated_available_campuses) | **GET** /tenants/{tenantId}/observations/campuses | Get Available Campuses
[**get_paginated_available_forms**](ObservationsApi.md#get_paginated_available_forms) | **GET** /tenants/{tenantId}/observations/available-forms | Get Paginated Available Forms
[**get_paginated_campus_sections**](ObservationsApi.md#get_paginated_campus_sections) | **GET** /tenants/{tenantId}/observations/campuses/{campusId}/sections | Retrieves a list of Sections for a given available campus.
[**get_paginated_campuses_with_evaluees**](ObservationsApi.md#get_paginated_campuses_with_evaluees) | **GET** /tenants/{tenantId}/observations/campuses-with-evaluees | Get a paginated list of the available campuses that have evaluees, each with its complete list of evaluees.
[**get_paginated_evaluees**](ObservationsApi.md#get_paginated_evaluees) | **GET** /tenants/{tenantId}/observations/evaluees | Get paginated evaluees
[**get_paginated_observation_users**](ObservationsApi.md#get_paginated_observation_users) | **GET** /tenants/{tenantId}/observations/users | Get paginated users for a given tenant, including their SEOAAs and Observation Access.
[**get_paginated_observations**](ObservationsApi.md#get_paginated_observations) | **GET** /tenants/{tenantId}/observations | Get Paginated Observations for a given tenant
[**get_paginated_observers**](ObservationsApi.md#get_paginated_observers) | **GET** /tenants/{tenantId}/observations/observers | Get paginated observers
[**get_sections_count**](ObservationsApi.md#get_sections_count) | **GET** /tenants/{tenantId}/observations/sectionscount | Gets the total count of sections for a given tenant
[**get_seoaas_total**](ObservationsApi.md#get_seoaas_total) | **GET** /tenants/{tenantId}/observations/seoaastotals | Get the total number of SEOAAs across all users for a given tenant
[**get_sessions_count**](ObservationsApi.md#get_sessions_count) | **GET** /tenants/{tenantId}/observations/sessionscount | Gets the total count of sessions for a given tenant
[**get_staff_section_associations_count**](ObservationsApi.md#get_staff_section_associations_count) | **GET** /tenants/{tenantId}/observations/staffsectionassociationscount | Gets the total count of staff-section associations across all users for a given tenant
[**get_submitted_observations_count**](ObservationsApi.md#get_submitted_observations_count) | **GET** /tenants/{tenantId}/submittedobservations | Get submitted Observations count
[**get_terms_count**](ObservationsApi.md#get_terms_count) | **GET** /tenants/{tenantId}/observations/termscount | Gets the total count of terms for a given tenant
[**get_user_sync_job**](ObservationsApi.md#get_user_sync_job) | **GET** /tenants/{tenantId}/observations/usersync | Gets the User Sync job for a given tenant, including its job executions
[**save_dashboard_preferences**](ObservationsApi.md#save_dashboard_preferences) | **POST** /tenants/{tenantId}/observations/dashboards/{dashboardId}/preferences | Save user preferences for a given Dashboard
[**search_paginated_evaluees**](ObservationsApi.md#search_paginated_evaluees) | **GET** /tenants/{tenantId}/observations/search/evaluees | Search paginated evaluees
[**update_observation**](ObservationsApi.md#update_observation) | **PUT** /tenants/{tenantId}/observations/{observationId} | Update an Observation for a given tenant
[**update_observations_onboarding_step**](ObservationsApi.md#update_observations_onboarding_step) | **PUT** /tenants/{tenantId}/observations/onboarding/{stepNumber} | Updates a step of the Instructional Insights onboarding for a given tenant
[**update_user_sync_job**](ObservationsApi.md#update_user_sync_job) | **PUT** /tenants/{tenantId}/observations/usersync | Updates the User Sync job for a given tenant
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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_services_observations_create_observation_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationRequest() # EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationRequest |  (optional)

    try:
        # Creates a new Observation for a given tenant
        api_response = await api_instance.create_observation(tenant_id, ed_graph_http_aggregators_tenant_api_services_observations_create_observation_request=ed_graph_http_aggregators_tenant_api_services_observations_create_observation_request)
        print("The response of ObservationsApi->create_observation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->create_observation: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    observation_id = 'observation_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_services_observations_create_observation_submission_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationSubmissionRequest() # EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationSubmissionRequest |  (optional)

    try:
        # Creates a submission for an available form referencing an existing observation
        api_response = await api_instance.create_observation_submission(tenant_id, form_id, observation_id, ed_graph_http_aggregators_tenant_api_services_observations_create_observation_submission_request=ed_graph_http_aggregators_tenant_api_services_observations_create_observation_submission_request)
        print("The response of ObservationsApi->create_observation_submission:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->create_observation_submission: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **form_id** | **UUID**|  | 
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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    observation_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Deletes an Observation for a given tenant
        api_response = await api_instance.delete_observation(tenant_id, observation_id)
        print("The response of ObservationsApi->delete_observation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->delete_observation: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **observation_id** | **UUID**|  | 

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

# **execute_user_sync_job**
> DataSyncApiJobV1JobExecutionRequestedResponse execute_user_sync_job(tenant_id)

Executes the User Sync job for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.data_sync_api_job_v1_job_execution_requested_response import DataSyncApiJobV1JobExecutionRequestedResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Executes the User Sync job for a given tenant
        api_response = await api_instance.execute_user_sync_job(tenant_id)
        print("The response of ObservationsApi->execute_user_sync_job:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->execute_user_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 

### Return type

[**DataSyncApiJobV1JobExecutionRequestedResponse**](DataSyncApiJobV1JobExecutionRequestedResponse.md)

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
**202** | The request has been accepted for processing, but the processing is not yet complete. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_academic_subjects_count**
> EdGraphHttpAggregatorsTenantApiServicesObservationsGetAcademicSubjectsCountResponse get_academic_subjects_count(tenant_id)

Gets the total count of academic subjects for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_get_academic_subjects_count_response import EdGraphHttpAggregatorsTenantApiServicesObservationsGetAcademicSubjectsCountResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets the total count of academic subjects for a given tenant
        api_response = await api_instance.get_academic_subjects_count(tenant_id)
        print("The response of ObservationsApi->get_academic_subjects_count:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_academic_subjects_count: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsGetAcademicSubjectsCountResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsGetAcademicSubjectsCountResponse.md)

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

# **get_available_campuses_total_evaluees**
> EdGraphHttpAggregatorsTenantApiServicesObservationsGetAvailableCampusesTotalEvalueesResponse get_available_campuses_total_evaluees(tenant_id)

Get the total number of evaluees across all available campuses

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_get_available_campuses_total_evaluees_response import EdGraphHttpAggregatorsTenantApiServicesObservationsGetAvailableCampusesTotalEvalueesResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Get the total number of evaluees across all available campuses
        api_response = await api_instance.get_available_campuses_total_evaluees(tenant_id)
        print("The response of ObservationsApi->get_available_campuses_total_evaluees:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_available_campuses_total_evaluees: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsGetAvailableCampusesTotalEvalueesResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsGetAvailableCampusesTotalEvalueesResponse.md)

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

# **get_courses_count**
> EdGraphHttpAggregatorsTenantApiServicesObservationsGetCoursesCountResponse get_courses_count(tenant_id)

Gets the total count of courses for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_get_courses_count_response import EdGraphHttpAggregatorsTenantApiServicesObservationsGetCoursesCountResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets the total count of courses for a given tenant
        api_response = await api_instance.get_courses_count(tenant_id)
        print("The response of ObservationsApi->get_courses_count:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_courses_count: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsGetCoursesCountResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsGetCoursesCountResponse.md)

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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    dashboard_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    persona_identifier = 'persona_identifier_example' # str |  (optional)

    try:
        # Get Observation Dashboard
        api_response = await api_instance.get_dashboard(tenant_id, dashboard_id, persona_identifier=persona_identifier)
        print("The response of ObservationsApi->get_dashboard:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_dashboard: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **dashboard_id** | **UUID**|  | 
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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    dashboard_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Save user preferences for a given Dashboard
        api_response = await api_instance.get_dashboard_preferences(tenant_id, dashboard_id)
        print("The response of ObservationsApi->get_dashboard_preferences:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_dashboard_preferences: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **dashboard_id** | **UUID**|  | 

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

# **get_default_ed_fi_instance**
> EdfiAdminApiEdfiAdminV1Instance get_default_ed_fi_instance(tenant_id)

Gets the default Ed-Fi instance for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance import EdfiAdminApiEdfiAdminV1Instance
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets the default Ed-Fi instance for a given tenant
        api_response = await api_instance.get_default_ed_fi_instance(tenant_id)
        print("The response of ObservationsApi->get_default_ed_fi_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_default_ed_fi_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 

### Return type

[**EdfiAdminApiEdfiAdminV1Instance**](EdfiAdminApiEdfiAdminV1Instance.md)

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

# **get_education_organizations_count**
> EdGraphHttpAggregatorsTenantApiServicesObservationsGetEducationOrganizationsCountResponse get_education_organizations_count(tenant_id, discriminator=discriminator)

Gets the total count of education organizations for a given tenant, filtered by discriminator

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_get_education_organizations_count_response import EdGraphHttpAggregatorsTenantApiServicesObservationsGetEducationOrganizationsCountResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    discriminator = 'discriminator_example' # str | Either \"LocalEducationAgency\" or \"School\" (optional)

    try:
        # Gets the total count of education organizations for a given tenant, filtered by discriminator
        api_response = await api_instance.get_education_organizations_count(tenant_id, discriminator=discriminator)
        print("The response of ObservationsApi->get_education_organizations_count:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_education_organizations_count: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **discriminator** | **str**| Either \&quot;LocalEducationAgency\&quot; or \&quot;School\&quot; | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsGetEducationOrganizationsCountResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsGetEducationOrganizationsCountResponse.md)

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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    evaluee_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter_by = '' # str |  (optional) (default to '')

    try:
        # Gets the Sections of an evaluee.
        api_response = await api_instance.get_evaluee_sections(tenant_id, evaluee_id, page_index=page_index, page_size=page_size, order_by=order_by, filter_by=filter_by)
        print("The response of ObservationsApi->get_evaluee_sections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_evaluee_sections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **evaluee_id** | **UUID**|  | 
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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    section_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)

    try:
        # Search Questions
        api_response = await api_instance.get_form_questions(tenant_id, form_id, section_id, page_index=page_index, page_size=page_size)
        print("The response of ObservationsApi->get_form_questions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_form_questions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **form_id** | **UUID**|  | 
 **section_id** | **UUID**|  | 
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
> FormApiSectionsV1SectionResponsePaginatedItemsViewModel get_form_sections(tenant_id, form_id, page_index=page_index, page_size=page_size)

Search Observation Form Sections

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.form_api_sections_v1_section_response_paginated_items_view_model import FormApiSectionsV1SectionResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)

    try:
        # Search Observation Form Sections
        api_response = await api_instance.get_form_sections(tenant_id, form_id, page_index=page_index, page_size=page_size)
        print("The response of ObservationsApi->get_form_sections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_form_sections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **form_id** | **UUID**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]

### Return type

[**FormApiSectionsV1SectionResponsePaginatedItemsViewModel**](FormApiSectionsV1SectionResponsePaginatedItemsViewModel.md)

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

# **get_grade_levels_count**
> EdGraphHttpAggregatorsTenantApiServicesObservationsGetGradeLevelsCountResponse get_grade_levels_count(tenant_id)

Gets the total count of grade levels for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_get_grade_levels_count_response import EdGraphHttpAggregatorsTenantApiServicesObservationsGetGradeLevelsCountResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets the total count of grade levels for a given tenant
        api_response = await api_instance.get_grade_levels_count(tenant_id)
        print("The response of ObservationsApi->get_grade_levels_count:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_grade_levels_count: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsGetGradeLevelsCountResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsGetGradeLevelsCountResponse.md)

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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    observation_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Get an Observation for a given tenant
        api_response = await api_instance.get_observation_by_id(tenant_id, observation_id)
        print("The response of ObservationsApi->get_observation_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_observation_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **observation_id** | **UUID**|  | 

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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    observation_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Get an observation form's draft
        api_response = await api_instance.get_observation_draft(tenant_id, observation_id, form_id)
        print("The response of ObservationsApi->get_observation_draft:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_observation_draft: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **observation_id** | **UUID**|  | 
 **form_id** | **UUID**|  | 

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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    observation_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets a submission for a specific observation
        api_response = await api_instance.get_observation_submission(tenant_id, observation_id, form_id)
        print("The response of ObservationsApi->get_observation_submission:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_observation_submission: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **observation_id** | **UUID**|  | 
 **form_id** | **UUID**|  | 

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

# **get_onboarding**
> EdGraphHttpAggregatorsTenantApiServicesObservationsObservationsOnboardingResponse get_onboarding(tenant_id)

Gets the Instructional Insights onboarding progress for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_observations_onboarding_response import EdGraphHttpAggregatorsTenantApiServicesObservationsObservationsOnboardingResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets the Instructional Insights onboarding progress for a given tenant
        api_response = await api_instance.get_onboarding(tenant_id)
        print("The response of ObservationsApi->get_onboarding:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_onboarding: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsObservationsOnboardingResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsObservationsOnboardingResponse.md)

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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    name_of_institution = '' # str |  (optional) (default to '')

    try:
        # Get Available Campuses
        api_response = await api_instance.get_paginated_available_campuses(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, name_of_institution=name_of_institution)
        print("The response of ObservationsApi->get_paginated_available_campuses:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_paginated_available_campuses: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
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
> EdGraphHttpAggregatorsTenantApiServicesFormsV1FormGetPaginatedItemsResponse get_paginated_available_forms(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)

Get Paginated Available Forms

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_forms_v1_form_get_paginated_items_response import EdGraphHttpAggregatorsTenantApiServicesFormsV1FormGetPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Get Paginated Available Forms
        api_response = await api_instance.get_paginated_available_forms(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)
        print("The response of ObservationsApi->get_paginated_available_forms:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_paginated_available_forms: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesFormsV1FormGetPaginatedItemsResponse**](EdGraphHttpAggregatorsTenantApiServicesFormsV1FormGetPaginatedItemsResponse.md)

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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    campus_id = 'campus_id_example' # str | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of Sections for a given available campus.
        api_response = await api_instance.get_paginated_campus_sections(tenant_id, campus_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter)
        print("The response of ObservationsApi->get_paginated_campus_sections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_paginated_campus_sections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
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

# **get_paginated_campuses_with_evaluees**
> EdGraphHttpAggregatorsTenantApiServicesObservationsGetCampusesWithEvalueesResponse get_paginated_campuses_with_evaluees(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by)

Get a paginated list of the available campuses that have evaluees, each with its complete list of evaluees.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_get_campuses_with_evaluees_response import EdGraphHttpAggregatorsTenantApiServicesObservationsGetCampusesWithEvalueesResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')

    try:
        # Get a paginated list of the available campuses that have evaluees, each with its complete list of evaluees.
        api_response = await api_instance.get_paginated_campuses_with_evaluees(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by)
        print("The response of ObservationsApi->get_paginated_campuses_with_evaluees:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_paginated_campuses_with_evaluees: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsGetCampusesWithEvalueesResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsGetCampusesWithEvalueesResponse.md)

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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    campus = '' # str |  (optional) (default to '')
    evaluee_id = '' # str |  (optional) (default to '')
    first_name = '' # str |  (optional) (default to '')
    last_name = '' # str |  (optional) (default to '')

    try:
        # Get paginated evaluees
        api_response = await api_instance.get_paginated_evaluees(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, campus=campus, evaluee_id=evaluee_id, first_name=first_name, last_name=last_name)
        print("The response of ObservationsApi->get_paginated_evaluees:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_paginated_evaluees: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
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

# **get_paginated_observation_users**
> EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserResponseGetPaginatedItemsResponse get_paginated_observation_users(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter, first_name=first_name, last_name=last_name, email=email, organization=organization, education_organization_role=education_organization_role, persona=persona)

Get paginated users for a given tenant, including their SEOAAs and Observation Access.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_observation_user_response_get_paginated_items_response import EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserResponseGetPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')
    first_name = '' # str |  (optional) (default to '')
    last_name = '' # str |  (optional) (default to '')
    email = '' # str |  (optional) (default to '')
    organization = '' # str |  (optional) (default to '')
    education_organization_role = '' # str |  (optional) (default to '')
    persona = '' # str |  (optional) (default to '')

    try:
        # Get paginated users for a given tenant, including their SEOAAs and Observation Access.
        api_response = await api_instance.get_paginated_observation_users(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, filter=filter, first_name=first_name, last_name=last_name, email=email, organization=organization, education_organization_role=education_organization_role, persona=persona)
        print("The response of ObservationsApi->get_paginated_observation_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_paginated_observation_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]
 **first_name** | **str**|  | [optional] [default to &#39;&#39;]
 **last_name** | **str**|  | [optional] [default to &#39;&#39;]
 **email** | **str**|  | [optional] [default to &#39;&#39;]
 **organization** | **str**|  | [optional] [default to &#39;&#39;]
 **education_organization_role** | **str**|  | [optional] [default to &#39;&#39;]
 **persona** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserResponseGetPaginatedItemsResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserResponseGetPaginatedItemsResponse.md)

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
> EdGraphHttpAggregatorsTenantApiServicesObservationsObservationProfileResponsePaginatedItemsViewModel get_paginated_observations(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, campus=campus, evaluee_name=evaluee_name, evaluee_id=evaluee_id, form_id=form_id, status=status, var_from=var_from, to=to, observer_id=observer_id)

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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
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
    observer_id = '' # str |  (optional) (default to '')

    try:
        # Get Paginated Observations for a given tenant
        api_response = await api_instance.get_paginated_observations(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, campus=campus, evaluee_name=evaluee_name, evaluee_id=evaluee_id, form_id=form_id, status=status, var_from=var_from, to=to, observer_id=observer_id)
        print("The response of ObservationsApi->get_paginated_observations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_paginated_observations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
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
 **observer_id** | **str**|  | [optional] [default to &#39;&#39;]

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

# **get_paginated_observers**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEvaluationsAppraiserResponseGetPaginatedItemsResponse get_paginated_observers(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Get paginated observers

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_evaluations_appraiser_response_get_paginated_items_response import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEvaluationsAppraiserResponseGetPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Get paginated observers
        api_response = await api_instance.get_paginated_observers(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of ObservationsApi->get_paginated_observers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_paginated_observers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEvaluationsAppraiserResponseGetPaginatedItemsResponse**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEvaluationsAppraiserResponseGetPaginatedItemsResponse.md)

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

# **get_sections_count**
> EdGraphHttpAggregatorsTenantApiServicesObservationsGetSectionsCountResponse get_sections_count(tenant_id)

Gets the total count of sections for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_get_sections_count_response import EdGraphHttpAggregatorsTenantApiServicesObservationsGetSectionsCountResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets the total count of sections for a given tenant
        api_response = await api_instance.get_sections_count(tenant_id)
        print("The response of ObservationsApi->get_sections_count:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_sections_count: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsGetSectionsCountResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsGetSectionsCountResponse.md)

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

# **get_seoaas_total**
> EdGraphHttpAggregatorsTenantApiServicesObservationsGetSeoaasTotalResponse get_seoaas_total(tenant_id)

Get the total number of SEOAAs across all users for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_get_seoaas_total_response import EdGraphHttpAggregatorsTenantApiServicesObservationsGetSeoaasTotalResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Get the total number of SEOAAs across all users for a given tenant
        api_response = await api_instance.get_seoaas_total(tenant_id)
        print("The response of ObservationsApi->get_seoaas_total:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_seoaas_total: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsGetSeoaasTotalResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsGetSeoaasTotalResponse.md)

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

# **get_sessions_count**
> EdGraphHttpAggregatorsTenantApiServicesObservationsGetSessionsCountResponse get_sessions_count(tenant_id)

Gets the total count of sessions for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_get_sessions_count_response import EdGraphHttpAggregatorsTenantApiServicesObservationsGetSessionsCountResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets the total count of sessions for a given tenant
        api_response = await api_instance.get_sessions_count(tenant_id)
        print("The response of ObservationsApi->get_sessions_count:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_sessions_count: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsGetSessionsCountResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsGetSessionsCountResponse.md)

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

# **get_staff_section_associations_count**
> EdGraphHttpAggregatorsTenantApiServicesObservationsGetStaffSectionAssociationsCountResponse get_staff_section_associations_count(tenant_id)

Gets the total count of staff-section associations across all users for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_get_staff_section_associations_count_response import EdGraphHttpAggregatorsTenantApiServicesObservationsGetStaffSectionAssociationsCountResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets the total count of staff-section associations across all users for a given tenant
        api_response = await api_instance.get_staff_section_associations_count(tenant_id)
        print("The response of ObservationsApi->get_staff_section_associations_count:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_staff_section_associations_count: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsGetStaffSectionAssociationsCountResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsGetStaffSectionAssociationsCountResponse.md)

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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    evaluee_id = 'evaluee_id_example' # str |  (optional)
    campus = 'campus_example' # str |  (optional)

    try:
        # Get submitted Observations count
        api_response = await api_instance.get_submitted_observations_count(tenant_id, evaluee_id=evaluee_id, campus=campus)
        print("The response of ObservationsApi->get_submitted_observations_count:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_submitted_observations_count: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
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

# **get_terms_count**
> EdGraphHttpAggregatorsTenantApiServicesObservationsGetTermsCountResponse get_terms_count(tenant_id)

Gets the total count of terms for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_get_terms_count_response import EdGraphHttpAggregatorsTenantApiServicesObservationsGetTermsCountResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets the total count of terms for a given tenant
        api_response = await api_instance.get_terms_count(tenant_id)
        print("The response of ObservationsApi->get_terms_count:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_terms_count: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsGetTermsCountResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsGetTermsCountResponse.md)

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

# **get_user_sync_job**
> EdGraphHttpAggregatorsTenantApiServicesObservationsUserSyncJobResponse get_user_sync_job(tenant_id)

Gets the User Sync job for a given tenant, including its job executions

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_user_sync_job_response import EdGraphHttpAggregatorsTenantApiServicesObservationsUserSyncJobResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets the User Sync job for a given tenant, including its job executions
        api_response = await api_instance.get_user_sync_job(tenant_id)
        print("The response of ObservationsApi->get_user_sync_job:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->get_user_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsUserSyncJobResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsUserSyncJobResponse.md)

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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    dashboard_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_services_observations_upsert_dashboard_preferences_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertDashboardPreferencesRequest() # EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertDashboardPreferencesRequest |  (optional)

    try:
        # Save user preferences for a given Dashboard
        api_response = await api_instance.save_dashboard_preferences(tenant_id, dashboard_id, ed_graph_http_aggregators_tenant_api_services_observations_upsert_dashboard_preferences_request=ed_graph_http_aggregators_tenant_api_services_observations_upsert_dashboard_preferences_request)
        print("The response of ObservationsApi->save_dashboard_preferences:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->save_dashboard_preferences: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **dashboard_id** | **UUID**|  | 
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

# **search_paginated_evaluees**
> EdGraphHttpAggregatorsTenantApiServicesObservationsEvalueeResponsePaginatedItemsViewModel search_paginated_evaluees(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, first_name=first_name, last_name=last_name)

Search paginated evaluees

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_evaluee_response_paginated_items_view_model import EdGraphHttpAggregatorsTenantApiServicesObservationsEvalueeResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    first_name = '' # str |  (optional) (default to '')
    last_name = '' # str |  (optional) (default to '')

    try:
        # Search paginated evaluees
        api_response = await api_instance.search_paginated_evaluees(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, first_name=first_name, last_name=last_name)
        print("The response of ObservationsApi->search_paginated_evaluees:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->search_paginated_evaluees: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **first_name** | **str**|  | [optional] [default to &#39;&#39;]
 **last_name** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsEvalueeResponsePaginatedItemsViewModel**](EdGraphHttpAggregatorsTenantApiServicesObservationsEvalueeResponsePaginatedItemsViewModel.md)

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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    observation_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_services_observations_update_observation_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationRequest() # EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationRequest |  (optional)

    try:
        # Update an Observation for a given tenant
        api_response = await api_instance.update_observation(tenant_id, observation_id, ed_graph_http_aggregators_tenant_api_services_observations_update_observation_request=ed_graph_http_aggregators_tenant_api_services_observations_update_observation_request)
        print("The response of ObservationsApi->update_observation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->update_observation: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **observation_id** | **UUID**|  | 
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

# **update_observations_onboarding_step**
> EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationsOnboardingStepResponse update_observations_onboarding_step(tenant_id, step_number, ed_graph_http_aggregators_tenant_api_services_observations_update_observations_onboarding_step_request=ed_graph_http_aggregators_tenant_api_services_observations_update_observations_onboarding_step_request)

Updates a step of the Instructional Insights onboarding for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_update_observations_onboarding_step_request import EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationsOnboardingStepRequest
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_update_observations_onboarding_step_response import EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationsOnboardingStepResponse
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    step_number = 56 # int | 
    ed_graph_http_aggregators_tenant_api_services_observations_update_observations_onboarding_step_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationsOnboardingStepRequest() # EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationsOnboardingStepRequest |  (optional)

    try:
        # Updates a step of the Instructional Insights onboarding for a given tenant
        api_response = await api_instance.update_observations_onboarding_step(tenant_id, step_number, ed_graph_http_aggregators_tenant_api_services_observations_update_observations_onboarding_step_request=ed_graph_http_aggregators_tenant_api_services_observations_update_observations_onboarding_step_request)
        print("The response of ObservationsApi->update_observations_onboarding_step:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->update_observations_onboarding_step: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **step_number** | **int**|  | 
 **ed_graph_http_aggregators_tenant_api_services_observations_update_observations_onboarding_step_request** | [**EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationsOnboardingStepRequest**](EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationsOnboardingStepRequest.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationsOnboardingStepResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationsOnboardingStepResponse.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_user_sync_job**
> MicrosoftAspNetCoreMvcNoContentResult update_user_sync_job(tenant_id, body=body)

Updates the User Sync job for a given tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.microsoft_asp_net_core_mvc_no_content_result import MicrosoftAspNetCoreMvcNoContentResult
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
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    body = None # object |  (optional)

    try:
        # Updates the User Sync job for a given tenant
        api_response = await api_instance.update_user_sync_job(tenant_id, body=body)
        print("The response of ObservationsApi->update_user_sync_job:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->update_user_sync_job: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **body** | **object**|  | [optional] 

### Return type

[**MicrosoftAspNetCoreMvcNoContentResult**](MicrosoftAspNetCoreMvcNoContentResult.md)

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
**204** | The resource was successfully updated. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |
**404** | The resource could not be found. |  -  |

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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    observation_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    form_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_services_observations_upsert_observation_draft_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertObservationDraftRequest() # EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertObservationDraftRequest |  (optional)

    try:
        # Creates a draft for an observation forms
        api_response = await api_instance.upsert_observation_draft(tenant_id, observation_id, form_id, ed_graph_http_aggregators_tenant_api_services_observations_upsert_observation_draft_request=ed_graph_http_aggregators_tenant_api_services_observations_upsert_observation_draft_request)
        print("The response of ObservationsApi->upsert_observation_draft:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->upsert_observation_draft: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **observation_id** | **UUID**|  | 
 **form_id** | **UUID**|  | 
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
async with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.ObservationsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_services_observations_use_cases_commands_dashboard_access_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesObservationsUseCasesCommandsDashboardAccessRequest() # EdGraphHttpAggregatorsTenantApiServicesObservationsUseCasesCommandsDashboardAccessRequest |  (optional)

    try:
        # Verify user access to dashboards
        api_response = await api_instance.verify_dashboard_access(tenant_id, ed_graph_http_aggregators_tenant_api_services_observations_use_cases_commands_dashboard_access_request=ed_graph_http_aggregators_tenant_api_services_observations_use_cases_commands_dashboard_access_request)
        print("The response of ObservationsApi->verify_dashboard_access:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ObservationsApi->verify_dashboard_access: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
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

