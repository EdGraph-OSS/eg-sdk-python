# edgraph_platform_client.EnrollmentAdminRegistrationsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_enrollment_registration_application**](EnrollmentAdminRegistrationsApi.md#add_enrollment_registration_application) | **POST** /tenants/{tenantId}/enrollmentadmin/registrations/{id}/applications | Adds one Program-seat choice to an existing Registration - the standalone counterpart to  passing initial choices at creation time.
[**approve_enrollment_registration**](EnrollmentAdminRegistrationsApi.md#approve_enrollment_registration) | **PUT** /tenants/{tenantId}/enrollmentadmin/registrations/{id}/approve | Approves a Registration - assigns the linked Student and Contacts and flips its status.
[**approve_enrollment_registration_application**](EnrollmentAdminRegistrationsApi.md#approve_enrollment_registration_application) | **PUT** /tenants/{tenantId}/enrollmentadmin/registrations/{id}/applications/{applicationId}/approve | Approves a single Application on a Registration, independently of its siblings.
[**create_enrollment_registration**](EnrollmentAdminRegistrationsApi.md#create_enrollment_registration) | **POST** /tenants/{tenantId}/enrollmentadmin/registrations | Creates a Registration.
[**delete_enrollment_registration**](EnrollmentAdminRegistrationsApi.md#delete_enrollment_registration) | **DELETE** /tenants/{tenantId}/enrollmentadmin/registrations/{id} | Removes a Registration.
[**get_enrollment_registration**](EnrollmentAdminRegistrationsApi.md#get_enrollment_registration) | **GET** /tenants/{tenantId}/enrollmentadmin/registrations/{id} | Gets a Registration by its id.
[**get_enrollment_registration_applications**](EnrollmentAdminRegistrationsApi.md#get_enrollment_registration_applications) | **GET** /tenants/{tenantId}/enrollmentadmin/registrations/{id}/applications | Gets a Registration&#39;s Applications - each a zero-to-many, independently approvable  Program-seat choice.
[**get_enrollment_registrations**](EnrollmentAdminRegistrationsApi.md#get_enrollment_registrations) | **GET** /tenants/{tenantId}/enrollmentadmin/registrations | Searches Registrations - a parent&#39;s enrollment submission requesting a seat in a School/District  Program.
[**reject_enrollment_registration**](EnrollmentAdminRegistrationsApi.md#reject_enrollment_registration) | **PUT** /tenants/{tenantId}/enrollmentadmin/registrations/{id}/reject | Explicitly rejects a Registration - sets its status to Rejected. Terminal, like approve: a  later Update/UpdateScreen/StartOver progress recompute does not revert it.
[**submit_enrollment_registration**](EnrollmentAdminRegistrationsApi.md#submit_enrollment_registration) | **PUT** /tenants/{tenantId}/enrollmentadmin/registrations/{id}/submit | Explicitly submits a Registration - sets its status to Submitted. Terminal, like approve: a  later Update/UpdateScreen/StartOver progress recompute does not revert it.
[**update_enrollment_registration**](EnrollmentAdminRegistrationsApi.md#update_enrollment_registration) | **PUT** /tenants/{tenantId}/enrollmentadmin/registrations/{id} | Updates a Registration.


# **add_enrollment_registration_application**
> EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse add_enrollment_registration_application(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_add_registration_application_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_add_registration_application_request_dto)

Adds one Program-seat choice to an existing Registration - the standalone counterpart to  passing initial choices at creation time.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_add_registration_application_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminAddRegistrationApplicationRequestDto
from edgraph_platform_client.models.enrollment_api_enrollment_registrations_v1_registration_response import EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse
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
    api_instance = edgraph_platform_client.EnrollmentAdminRegistrationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = 'id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_add_registration_application_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminAddRegistrationApplicationRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminAddRegistrationApplicationRequestDto |  (optional)

    try:
        # Adds one Program-seat choice to an existing Registration - the standalone counterpart to  passing initial choices at creation time.
        api_response = await api_instance.add_enrollment_registration_application(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_add_registration_application_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_add_registration_application_request_dto)
        print("The response of EnrollmentAdminRegistrationsApi->add_enrollment_registration_application:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminRegistrationsApi->add_enrollment_registration_application: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_add_registration_application_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminAddRegistrationApplicationRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminAddRegistrationApplicationRequestDto.md)|  | [optional] 

### Return type

[**EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse**](EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The application was added. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **approve_enrollment_registration**
> EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse approve_enrollment_registration(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_registration_approve_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_registration_approve_request_dto)

Approves a Registration - assigns the linked Student and Contacts and flips its status.

The `contacts` array replaces/merges into the Registration's existing Contacts collection,
matched by `contactId` (upsert semantics) - there is no separate scalar contactId field.
The `choices` array sets the status of the Registration's Applications; each Application is
independently approvable - see the `applications/{applicationId}/approve` route to approve
just one without touching the others.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_registration_approve_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminRegistrationApproveRequestDto
from edgraph_platform_client.models.enrollment_api_enrollment_registrations_v1_registration_response import EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse
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
    api_instance = edgraph_platform_client.EnrollmentAdminRegistrationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = 'id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_registration_approve_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminRegistrationApproveRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminRegistrationApproveRequestDto |  (optional)

    try:
        # Approves a Registration - assigns the linked Student and Contacts and flips its status.
        api_response = await api_instance.approve_enrollment_registration(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_registration_approve_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_registration_approve_request_dto)
        print("The response of EnrollmentAdminRegistrationsApi->approve_enrollment_registration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminRegistrationsApi->approve_enrollment_registration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_registration_approve_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminRegistrationApproveRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminRegistrationApproveRequestDto.md)|  | [optional] 

### Return type

[**EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse**](EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The registration was approved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **approve_enrollment_registration_application**
> EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse approve_enrollment_registration_application(tenant_id, id, application_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_registration_approve_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_registration_approve_request_dto)

Approves a single Application on a Registration, independently of its siblings.

Same request body shape as `PUT .../registrations/{id}/approve`. Future Phase 99:
`PUT .../registrations/{id}/contacts/{id}/match` is out of scope and not implemented here.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_registration_approve_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminRegistrationApproveRequestDto
from edgraph_platform_client.models.enrollment_api_enrollment_registrations_v1_registration_response import EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse
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
    api_instance = edgraph_platform_client.EnrollmentAdminRegistrationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = 'id_example' # str | 
    application_id = 'application_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_registration_approve_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminRegistrationApproveRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminRegistrationApproveRequestDto |  (optional)

    try:
        # Approves a single Application on a Registration, independently of its siblings.
        api_response = await api_instance.approve_enrollment_registration_application(tenant_id, id, application_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_registration_approve_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_registration_approve_request_dto)
        print("The response of EnrollmentAdminRegistrationsApi->approve_enrollment_registration_application:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminRegistrationsApi->approve_enrollment_registration_application: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **str**|  | 
 **application_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_registration_approve_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminRegistrationApproveRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminRegistrationApproveRequestDto.md)|  | [optional] 

### Return type

[**EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse**](EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The application was approved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_enrollment_registration**
> EnrollmentApiEnrollmentRegistrationsV1RegistrationCreatedResponse create_enrollment_registration(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_registration_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_registration_request_dto)

Creates a Registration.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_registration_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateRegistrationRequestDto
from edgraph_platform_client.models.enrollment_api_enrollment_registrations_v1_registration_created_response import EnrollmentApiEnrollmentRegistrationsV1RegistrationCreatedResponse
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
    api_instance = edgraph_platform_client.EnrollmentAdminRegistrationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_registration_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateRegistrationRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateRegistrationRequestDto |  (optional)

    try:
        # Creates a Registration.
        api_response = await api_instance.create_enrollment_registration(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_registration_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_registration_request_dto)
        print("The response of EnrollmentAdminRegistrationsApi->create_enrollment_registration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminRegistrationsApi->create_enrollment_registration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_registration_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateRegistrationRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateRegistrationRequestDto.md)|  | [optional] 

### Return type

[**EnrollmentApiEnrollmentRegistrationsV1RegistrationCreatedResponse**](EnrollmentApiEnrollmentRegistrationsV1RegistrationCreatedResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**201** | The registration was created. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_enrollment_registration**
> delete_enrollment_registration(tenant_id, id)

Removes a Registration.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
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
    api_instance = edgraph_platform_client.EnrollmentAdminRegistrationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = 'id_example' # str | 

    try:
        # Removes a Registration.
        await api_instance.delete_enrollment_registration(tenant_id, id)
    except Exception as e:
        print("Exception when calling EnrollmentAdminRegistrationsApi->delete_enrollment_registration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **str**|  | 

### Return type

void (empty response body)

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
**204** | The registration was removed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_enrollment_registration**
> EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse get_enrollment_registration(tenant_id, id)

Gets a Registration by its id.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.enrollment_api_enrollment_registrations_v1_registration_response import EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse
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
    api_instance = edgraph_platform_client.EnrollmentAdminRegistrationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = 'id_example' # str | 

    try:
        # Gets a Registration by its id.
        api_response = await api_instance.get_enrollment_registration(tenant_id, id)
        print("The response of EnrollmentAdminRegistrationsApi->get_enrollment_registration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminRegistrationsApi->get_enrollment_registration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **str**|  | 

### Return type

[**EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse**](EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse.md)

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

# **get_enrollment_registration_applications**
> EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationsListResponse get_enrollment_registration_applications(tenant_id, id)

Gets a Registration's Applications - each a zero-to-many, independently approvable  Program-seat choice.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.enrollment_api_enrollment_registrations_v1_registration_applications_list_response import EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationsListResponse
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
    api_instance = edgraph_platform_client.EnrollmentAdminRegistrationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = 'id_example' # str | 

    try:
        # Gets a Registration's Applications - each a zero-to-many, independently approvable  Program-seat choice.
        api_response = await api_instance.get_enrollment_registration_applications(tenant_id, id)
        print("The response of EnrollmentAdminRegistrationsApi->get_enrollment_registration_applications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminRegistrationsApi->get_enrollment_registration_applications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **str**|  | 

### Return type

[**EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationsListResponse**](EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationsListResponse.md)

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

# **get_enrollment_registrations**
> EnrollmentApiEnrollmentRegistrationsV1RegistrationsSearchResponse get_enrollment_registrations(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)

Searches Registrations - a parent's enrollment submission requesting a seat in a School/District  Program.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.enrollment_api_enrollment_registrations_v1_registrations_search_response import EnrollmentApiEnrollmentRegistrationsV1RegistrationsSearchResponse
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
    api_instance = edgraph_platform_client.EnrollmentAdminRegistrationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_index = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    filter = 'filter_example' # str |  (optional)
    order_by = 'order_by_example' # str |  (optional)

    try:
        # Searches Registrations - a parent's enrollment submission requesting a seat in a School/District  Program.
        api_response = await api_instance.get_enrollment_registrations(tenant_id, page_index=page_index, page_size=page_size, filter=filter, order_by=order_by)
        print("The response of EnrollmentAdminRegistrationsApi->get_enrollment_registrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminRegistrationsApi->get_enrollment_registrations: %s\n" % e)
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

[**EnrollmentApiEnrollmentRegistrationsV1RegistrationsSearchResponse**](EnrollmentApiEnrollmentRegistrationsV1RegistrationsSearchResponse.md)

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

# **reject_enrollment_registration**
> EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse reject_enrollment_registration(tenant_id, id, body=body)

Explicitly rejects a Registration - sets its status to Rejected. Terminal, like approve: a  later Update/UpdateScreen/StartOver progress recompute does not revert it.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.enrollment_api_enrollment_registrations_v1_registration_response import EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse
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
    api_instance = edgraph_platform_client.EnrollmentAdminRegistrationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = 'id_example' # str | 
    body = None # object |  (optional)

    try:
        # Explicitly rejects a Registration - sets its status to Rejected. Terminal, like approve: a  later Update/UpdateScreen/StartOver progress recompute does not revert it.
        api_response = await api_instance.reject_enrollment_registration(tenant_id, id, body=body)
        print("The response of EnrollmentAdminRegistrationsApi->reject_enrollment_registration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminRegistrationsApi->reject_enrollment_registration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **str**|  | 
 **body** | **object**|  | [optional] 

### Return type

[**EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse**](EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The registration was rejected. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **submit_enrollment_registration**
> EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse submit_enrollment_registration(tenant_id, id, body=body)

Explicitly submits a Registration - sets its status to Submitted. Terminal, like approve: a  later Update/UpdateScreen/StartOver progress recompute does not revert it.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.enrollment_api_enrollment_registrations_v1_registration_response import EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse
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
    api_instance = edgraph_platform_client.EnrollmentAdminRegistrationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = 'id_example' # str | 
    body = None # object |  (optional)

    try:
        # Explicitly submits a Registration - sets its status to Submitted. Terminal, like approve: a  later Update/UpdateScreen/StartOver progress recompute does not revert it.
        api_response = await api_instance.submit_enrollment_registration(tenant_id, id, body=body)
        print("The response of EnrollmentAdminRegistrationsApi->submit_enrollment_registration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminRegistrationsApi->submit_enrollment_registration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **str**|  | 
 **body** | **object**|  | [optional] 

### Return type

[**EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse**](EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The registration was submitted. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_enrollment_registration**
> EnrollmentApiEnrollmentRegistrationsV1RegistrationUpdatedResponse update_enrollment_registration(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_registration_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_registration_request_dto)

Updates a Registration.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_registration_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateRegistrationRequestDto
from edgraph_platform_client.models.enrollment_api_enrollment_registrations_v1_registration_updated_response import EnrollmentApiEnrollmentRegistrationsV1RegistrationUpdatedResponse
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
    api_instance = edgraph_platform_client.EnrollmentAdminRegistrationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = 'id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_registration_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateRegistrationRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateRegistrationRequestDto |  (optional)

    try:
        # Updates a Registration.
        api_response = await api_instance.update_enrollment_registration(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_registration_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_registration_request_dto)
        print("The response of EnrollmentAdminRegistrationsApi->update_enrollment_registration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminRegistrationsApi->update_enrollment_registration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_registration_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateRegistrationRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateRegistrationRequestDto.md)|  | [optional] 

### Return type

[**EnrollmentApiEnrollmentRegistrationsV1RegistrationUpdatedResponse**](EnrollmentApiEnrollmentRegistrationsV1RegistrationUpdatedResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The registration was updated. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

