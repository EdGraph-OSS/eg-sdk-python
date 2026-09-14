# edgraph_platform_client.EnrollmentAdminContactsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_enrollment_contact**](EnrollmentAdminContactsApi.md#create_enrollment_contact) | **POST** /tenants/{tenantId}/enrollmentadmin/contacts | Creates an Enrollment Contact.
[**get_enrollment_contact_by_id**](EnrollmentAdminContactsApi.md#get_enrollment_contact_by_id) | **GET** /tenants/{tenantId}/enrollmentadmin/contacts/{id} | Gets an Enrollment Contact by its record id, with its linked students.
[**get_enrollment_contact_overrides**](EnrollmentAdminContactsApi.md#get_enrollment_contact_overrides) | **GET** /tenants/{tenantId}/enrollmentadmin/contacts/{id}/overrides | Reads a contact&#39;s override history, newest first.
[**get_enrollment_contacts**](EnrollmentAdminContactsApi.md#get_enrollment_contacts) | **GET** /tenants/{tenantId}/enrollmentadmin/contacts | Searches Enrollment Contacts.
[**override_enrollment_contact_email**](EnrollmentAdminContactsApi.md#override_enrollment_contact_email) | **PUT** /tenants/{tenantId}/enrollmentadmin/contacts/{id}/email-override | Overrides a contact&#39;s email address.
[**override_enrollment_contact_phone**](EnrollmentAdminContactsApi.md#override_enrollment_contact_phone) | **PUT** /tenants/{tenantId}/enrollmentadmin/contacts/{id}/phone-override | Overrides a contact&#39;s phone number.
[**remove_enrollment_contact_email_override**](EnrollmentAdminContactsApi.md#remove_enrollment_contact_email_override) | **DELETE** /tenants/{tenantId}/enrollmentadmin/contacts/{id}/email-override | Removes a contact&#39;s email override, letting the SIS value show through again.
[**remove_enrollment_contact_phone_override**](EnrollmentAdminContactsApi.md#remove_enrollment_contact_phone_override) | **DELETE** /tenants/{tenantId}/enrollmentadmin/contacts/{id}/phone-override | Removes a contact&#39;s phone override, letting the SIS value show through again.
[**unlock_enrollment_contact_sign_in**](EnrollmentAdminContactsApi.md#unlock_enrollment_contact_sign_in) | **POST** /tenants/{tenantId}/enrollmentadmin/contacts/{id}/unlock | Unlocks a contact&#39;s sign-in, resetting exhausted parent-verification tries.
[**update_enrollment_contact**](EnrollmentAdminContactsApi.md#update_enrollment_contact) | **PUT** /tenants/{tenantId}/enrollmentadmin/contacts/{id} | Updates an Enrollment Contact name and its linked students.


# **create_enrollment_contact**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactMutationResultDto create_enrollment_contact(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_contact_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_contact_request_dto)

Creates an Enrollment Contact.

`email` and `phone` here are the SIS-sourced values, which is what a contact starts
            with. Changing either afterwards is an override rather than an update - see the
            `email-override` and `phone-override` routes.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_contact_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateContactRequestDto
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_mutation_result_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactMutationResultDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminContactsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_contact_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateContactRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateContactRequestDto |  (optional)

    try:
        # Creates an Enrollment Contact.
        api_response = await api_instance.create_enrollment_contact(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_contact_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_contact_request_dto)
        print("The response of EnrollmentAdminContactsApi->create_enrollment_contact:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminContactsApi->create_enrollment_contact: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_contact_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateContactRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateContactRequestDto.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactMutationResultDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactMutationResultDto.md)

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
**201** | The contact was created. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_enrollment_contact_by_id**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactResponseDto get_enrollment_contact_by_id(tenant_id, id)

Gets an Enrollment Contact by its record id, with its linked students.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_response_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactResponseDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminContactsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets an Enrollment Contact by its record id, with its linked students.
        api_response = await api_instance.get_enrollment_contact_by_id(tenant_id, id)
        print("The response of EnrollmentAdminContactsApi->get_enrollment_contact_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminContactsApi->get_enrollment_contact_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactResponseDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactResponseDto.md)

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

# **get_enrollment_contact_overrides**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideHistoryEntryDtoPaginatedItemsViewModel get_enrollment_contact_overrides(tenant_id, id, page_size=page_size, page_index=page_index, student_id=student_id)

Reads a contact's override history, newest first.

<br>
            Eventually consistent. A change reaches the log through Enrollment's outbox, so an entry can
            be a few seconds behind a write that has already succeeded. Render the current value from the
            contact itself and use this for what preceded it.
            
<br>
            One route for both details, unlike the writes: this is a single ordered log and each entry
            names its own detail, so splitting it would mean two requests to render one contact's
            timeline and two page counts to reconcile.
            

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_override_history_entry_dto_paginated_items_view_model import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideHistoryEntryDtoPaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.EnrollmentAdminContactsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_size = 20 # int |  (optional) (default to 20)
    page_index = 0 # int |  (optional) (default to 0)
    student_id = '' # str | Narrows to changes affecting one linked student. (optional) (default to '')

    try:
        # Reads a contact's override history, newest first.
        api_response = await api_instance.get_enrollment_contact_overrides(tenant_id, id, page_size=page_size, page_index=page_index, student_id=student_id)
        print("The response of EnrollmentAdminContactsApi->get_enrollment_contact_overrides:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminContactsApi->get_enrollment_contact_overrides: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 
 **page_size** | **int**|  | [optional] [default to 20]
 **page_index** | **int**|  | [optional] [default to 0]
 **student_id** | **str**| Narrows to changes affecting one linked student. | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideHistoryEntryDtoPaginatedItemsViewModel**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideHistoryEntryDtoPaginatedItemsViewModel.md)

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
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_enrollment_contacts**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactResponseDtoPaginatedItemsViewModel get_enrollment_contacts(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter, search=search, school_code=school_code, locked=locked)

Searches Enrollment Contacts.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_response_dto_paginated_items_view_model import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactResponseDtoPaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.EnrollmentAdminContactsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 50 # int |  (optional) (default to 50)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')
    search = '' # str | Free-text match on contact name, email, or phone. (optional) (default to '')
    school_code = '' # str | Narrows to contacts with at least one linked student at this school. (optional) (default to '')
    locked = True # bool | Narrows to contacts by sign-in lock status. Unset returns every contact. (optional)

    try:
        # Searches Enrollment Contacts.
        api_response = await api_instance.get_enrollment_contacts(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter, search=search, school_code=school_code, locked=locked)
        print("The response of EnrollmentAdminContactsApi->get_enrollment_contacts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminContactsApi->get_enrollment_contacts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 50]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]
 **search** | **str**| Free-text match on contact name, email, or phone. | [optional] [default to &#39;&#39;]
 **school_code** | **str**| Narrows to contacts with at least one linked student at this school. | [optional] [default to &#39;&#39;]
 **locked** | **bool**| Narrows to contacts by sign-in lock status. Unset returns every contact. | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactResponseDtoPaginatedItemsViewModel**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactResponseDtoPaginatedItemsViewModel.md)

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
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **override_enrollment_contact_email**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideResultDto override_enrollment_contact_email(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_email_override_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_email_override_request_dto)

Overrides a contact's email address.

The override is an enrollment-local annotation over SIS data, not a writeback. The SIS value
is kept and returned alongside it, and the correction keeps winning over later SIS imports
until staff revisit it.
<br>
The corrected value is shared by every student linked to the contact. `studentId` in the
body only records whose screen the edit came from.


### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_email_override_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactEmailOverrideRequestDto
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_override_result_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideResultDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminContactsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_email_override_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactEmailOverrideRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactEmailOverrideRequestDto |  (optional)

    try:
        # Overrides a contact's email address.
        api_response = await api_instance.override_enrollment_contact_email(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_email_override_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_email_override_request_dto)
        print("The response of EnrollmentAdminContactsApi->override_enrollment_contact_email:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminContactsApi->override_enrollment_contact_email: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_email_override_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactEmailOverrideRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactEmailOverrideRequestDto.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideResultDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideResultDto.md)

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
**200** | The override was applied. |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |
**412** | The contact changed while it was being edited; the write was refused. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **override_enrollment_contact_phone**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideResultDto override_enrollment_contact_phone(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_phone_override_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_phone_override_request_dto)

Overrides a contact's phone number.

The override is an enrollment-local annotation over SIS data, not a writeback. The SIS value
is kept and returned alongside it, and the correction keeps winning over later SIS imports
until staff revisit it.
<br>
The corrected value is shared by every student linked to the contact. `studentId` in the
body only records whose screen the edit came from.


### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_override_result_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideResultDto
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_phone_override_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactPhoneOverrideRequestDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminContactsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_phone_override_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactPhoneOverrideRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactPhoneOverrideRequestDto |  (optional)

    try:
        # Overrides a contact's phone number.
        api_response = await api_instance.override_enrollment_contact_phone(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_phone_override_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_phone_override_request_dto)
        print("The response of EnrollmentAdminContactsApi->override_enrollment_contact_phone:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminContactsApi->override_enrollment_contact_phone: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_phone_override_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactPhoneOverrideRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactPhoneOverrideRequestDto.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideResultDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideResultDto.md)

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
**200** | The override was applied. |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |
**412** | The contact changed while it was being edited; the write was refused. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **remove_enrollment_contact_email_override**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideResultDto remove_enrollment_contact_email_override(tenant_id, id, student_id=student_id, expected_version=expected_version)

Removes a contact's email override, letting the SIS value show through again.

The removal is itself recorded in the history - the superseded value stays recoverable.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_override_result_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideResultDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminContactsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    student_id = '' # str | The student whose screen the removal was made from. (optional) (default to '')
    expected_version = '' # str | The `lastUpdatedDateTime` this edit started from. (optional) (default to '')

    try:
        # Removes a contact's email override, letting the SIS value show through again.
        api_response = await api_instance.remove_enrollment_contact_email_override(tenant_id, id, student_id=student_id, expected_version=expected_version)
        print("The response of EnrollmentAdminContactsApi->remove_enrollment_contact_email_override:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminContactsApi->remove_enrollment_contact_email_override: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 
 **student_id** | **str**| The student whose screen the removal was made from. | [optional] [default to &#39;&#39;]
 **expected_version** | **str**| The &#x60;lastUpdatedDateTime&#x60; this edit started from. | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideResultDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideResultDto.md)

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
**200** | The override was removed, or there was none to remove. |  -  |
**404** | Not Found |  -  |
**412** | The contact changed while it was being edited; the write was refused. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **remove_enrollment_contact_phone_override**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideResultDto remove_enrollment_contact_phone_override(tenant_id, id, student_id=student_id, expected_version=expected_version)

Removes a contact's phone override, letting the SIS value show through again.

The removal is itself recorded in the history - the superseded value stays recoverable.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_override_result_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideResultDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminContactsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    student_id = '' # str | The student whose screen the removal was made from. (optional) (default to '')
    expected_version = '' # str | The `lastUpdatedDateTime` this edit started from. (optional) (default to '')

    try:
        # Removes a contact's phone override, letting the SIS value show through again.
        api_response = await api_instance.remove_enrollment_contact_phone_override(tenant_id, id, student_id=student_id, expected_version=expected_version)
        print("The response of EnrollmentAdminContactsApi->remove_enrollment_contact_phone_override:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminContactsApi->remove_enrollment_contact_phone_override: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 
 **student_id** | **str**| The student whose screen the removal was made from. | [optional] [default to &#39;&#39;]
 **expected_version** | **str**| The &#x60;lastUpdatedDateTime&#x60; this edit started from. | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideResultDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactOverrideResultDto.md)

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
**200** | The override was removed, or there was none to remove. |  -  |
**404** | Not Found |  -  |
**412** | The contact changed while it was being edited; the write was refused. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **unlock_enrollment_contact_sign_in**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactSignInUnlockedResultDto unlock_enrollment_contact_sign_in(tenant_id, id)

Unlocks a contact's sign-in, resetting exhausted parent-verification tries.

Idempotent: unlocking an already-unlocked contact, or one with no rows at all, is a 200 with
`resetCount: 0`, not an error.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_sign_in_unlocked_result_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactSignInUnlockedResultDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminContactsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Unlocks a contact's sign-in, resetting exhausted parent-verification tries.
        api_response = await api_instance.unlock_enrollment_contact_sign_in(tenant_id, id)
        print("The response of EnrollmentAdminContactsApi->unlock_enrollment_contact_sign_in:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminContactsApi->unlock_enrollment_contact_sign_in: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactSignInUnlockedResultDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactSignInUnlockedResultDto.md)

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
**200** | The contact&#39;s sign-in was unlocked, or there was nothing to unlock. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_enrollment_contact**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactMutationResultDto update_enrollment_contact(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_contact_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_contact_request_dto)

Updates an Enrollment Contact name and its linked students.

<br>
            The student list is REPLACED, not merged: a student omitted from the body is unlinked from the
            contact.
            
<br>
            Email and phone cannot be changed here. Correcting either is an override, which records who
            changed it and keeps the SIS value beside the correction; a body carrying `email` or
            `phone` is rejected with a 400 naming the route to use instead. Note that a contact whose
            email is overridden keeps that override across this call - an update to the name leaves a
            standing correction alone.
            

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_contact_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateContactRequestDto
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_contact_mutation_result_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactMutationResultDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminContactsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_contact_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateContactRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateContactRequestDto |  (optional)

    try:
        # Updates an Enrollment Contact name and its linked students.
        api_response = await api_instance.update_enrollment_contact(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_contact_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_contact_request_dto)
        print("The response of EnrollmentAdminContactsApi->update_enrollment_contact:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminContactsApi->update_enrollment_contact: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_contact_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateContactRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateContactRequestDto.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactMutationResultDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminContactMutationResultDto.md)

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
**200** | The contact was updated. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

