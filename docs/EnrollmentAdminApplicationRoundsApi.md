# edgraph_platform_client.EnrollmentAdminApplicationRoundsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_application_round_window**](EnrollmentAdminApplicationRoundsApi.md#add_application_round_window) | **POST** /tenants/{tenantId}/enrollmentadmin/applicationrounds/{id}/windows | Adds a window to the round. Windows may overlap, within the round and across rounds. A  dependency must name a window of a live round in the tenant.
[**create_application_round**](EnrollmentAdminApplicationRoundsApi.md#create_application_round) | **POST** /tenants/{tenantId}/enrollmentadmin/applicationrounds | Creates a round. Add its windows afterwards.
[**delete_application_round**](EnrollmentAdminApplicationRoundsApi.md#delete_application_round) | **DELETE** /tenants/{tenantId}/enrollmentadmin/applicationrounds/{id} | Soft-deletes a round. Refused once the round has opened, and while another round&#39;s window  depends on one of its windows.
[**duplicate_application_round**](EnrollmentAdminApplicationRoundsApi.md#duplicate_application_round) | **POST** /tenants/{tenantId}/enrollmentadmin/applicationrounds/{id}/duplicate | Copies the round&#39;s code, label, grades and program types into another school year. Windows  are not copied - their dates belong to this round&#39;s school year.
[**get_application_round_by_id**](EnrollmentAdminApplicationRoundsApi.md#get_application_round_by_id) | **GET** /tenants/{tenantId}/enrollmentadmin/applicationrounds/{id} | Gets a round by id, with its windows and their states as of now.
[**get_application_rounds**](EnrollmentAdminApplicationRoundsApi.md#get_application_rounds) | **GET** /tenants/{tenantId}/enrollmentadmin/applicationrounds | Searches the tenant&#39;s application rounds. Default order is school year descending, then code;  &#x60;orderBy&#x60; accepts &#x60;schoolYear&#x60; or &#x60;code&#x60;. Each round carries its windows and  the state of each, derived at the moment of the read.
[**purge_application_round**](EnrollmentAdminApplicationRoundsApi.md#purge_application_round) | **DELETE** /tenants/{tenantId}/enrollmentadmin/applicationrounds/{id}/purge | Hard-deletes a round. Only a round that has been deleted first.
[**recover_application_round**](EnrollmentAdminApplicationRoundsApi.md#recover_application_round) | **POST** /tenants/{tenantId}/enrollmentadmin/applicationrounds/{id}/recover | Brings back a soft-deleted round.
[**remove_application_round_window**](EnrollmentAdminApplicationRoundsApi.md#remove_application_round_window) | **DELETE** /tenants/{tenantId}/enrollmentadmin/applicationrounds/{id}/windows/{windowId} | Removes one window of the round. Refused while another window depends on it, and when it is  the last window of a round that has opened.
[**update_application_round**](EnrollmentAdminApplicationRoundsApi.md#update_application_round) | **PUT** /tenants/{tenantId}/enrollmentadmin/applicationrounds/{id} | Replaces a round&#39;s label, grades and program types. Code and school year never change -  duplicate the round into another school year instead.
[**update_application_round_window**](EnrollmentAdminApplicationRoundsApi.md#update_application_round_window) | **PUT** /tenants/{tenantId}/enrollmentadmin/applicationrounds/{id}/windows/{windowId} | Replaces one window of the round.


# **add_application_round_window**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundWindowMutationResultDto add_application_round_window(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto)

Adds a window to the round. Windows may overlap, within the round and across rounds. A  dependency must name a window of a live round in the tenant.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminEnrollmentWindowRequestDto
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_application_round_window_mutation_result_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundWindowMutationResultDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminApplicationRoundsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminEnrollmentWindowRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminEnrollmentWindowRequestDto |  (optional)

    try:
        # Adds a window to the round. Windows may overlap, within the round and across rounds. A  dependency must name a window of a live round in the tenant.
        api_response = await api_instance.add_application_round_window(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto)
        print("The response of EnrollmentAdminApplicationRoundsApi->add_application_round_window:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminApplicationRoundsApi->add_application_round_window: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminEnrollmentWindowRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminEnrollmentWindowRequestDto.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundWindowMutationResultDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundWindowMutationResultDto.md)

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
**201** | The window was added; the location is the round. |  -  |
**400** | Bad Request. The window was invalid, or its dependency names a window that does not exist. |  -  |
**404** | The resource could not be found. |  -  |
**412** | The dependency would make windows wait on each other in a loop. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_application_round**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundMutationResultDto create_application_round(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_application_round_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_application_round_request_dto)

Creates a round. Add its windows afterwards.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_application_round_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateApplicationRoundRequestDto
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_application_round_mutation_result_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundMutationResultDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminApplicationRoundsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_application_round_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateApplicationRoundRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateApplicationRoundRequestDto |  (optional)

    try:
        # Creates a round. Add its windows afterwards.
        api_response = await api_instance.create_application_round(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_application_round_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_application_round_request_dto)
        print("The response of EnrollmentAdminApplicationRoundsApi->create_application_round:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminApplicationRoundsApi->create_application_round: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_application_round_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateApplicationRoundRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateApplicationRoundRequestDto.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundMutationResultDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundMutationResultDto.md)

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
**201** | The round was created. |  -  |
**400** | Bad Request. The request was invalid, or named a program type that does not exist. |  -  |
**409** | The school year already has a round with this code, possibly deleted (recover or purge it first). |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_application_round**
> delete_application_round(tenant_id, id)

Soft-deletes a round. Refused once the round has opened, and while another round's window  depends on one of its windows.

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
    api_instance = edgraph_platform_client.EnrollmentAdminApplicationRoundsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Soft-deletes a round. Refused once the round has opened, and while another round's window  depends on one of its windows.
        await api_instance.delete_application_round(tenant_id, id)
    except Exception as e:
        print("Exception when calling EnrollmentAdminApplicationRoundsApi->delete_application_round: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 

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
**204** | The round was removed. |  -  |
**404** | The resource could not be found. |  -  |
**412** | The round has opened, or another window depends on it. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **duplicate_application_round**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundMutationResultDto duplicate_application_round(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_duplicate_application_round_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_duplicate_application_round_request_dto)

Copies the round's code, label, grades and program types into another school year. Windows  are not copied - their dates belong to this round's school year.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_duplicate_application_round_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminDuplicateApplicationRoundRequestDto
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_application_round_mutation_result_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundMutationResultDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminApplicationRoundsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_duplicate_application_round_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminDuplicateApplicationRoundRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminDuplicateApplicationRoundRequestDto |  (optional)

    try:
        # Copies the round's code, label, grades and program types into another school year. Windows  are not copied - their dates belong to this round's school year.
        api_response = await api_instance.duplicate_application_round(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_duplicate_application_round_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_duplicate_application_round_request_dto)
        print("The response of EnrollmentAdminApplicationRoundsApi->duplicate_application_round:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminApplicationRoundsApi->duplicate_application_round: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_duplicate_application_round_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminDuplicateApplicationRoundRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminDuplicateApplicationRoundRequestDto.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundMutationResultDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundMutationResultDto.md)

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
**201** | The copy was created. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |
**404** | The resource could not be found. |  -  |
**409** | That school year already has a round with this code, possibly deleted. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_application_round_by_id**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundResponseDto get_application_round_by_id(tenant_id, id)

Gets a round by id, with its windows and their states as of now.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_application_round_response_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundResponseDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminApplicationRoundsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets a round by id, with its windows and their states as of now.
        api_response = await api_instance.get_application_round_by_id(tenant_id, id)
        print("The response of EnrollmentAdminApplicationRoundsApi->get_application_round_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminApplicationRoundsApi->get_application_round_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundResponseDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundResponseDto.md)

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

# **get_application_rounds**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundResponseDtoPaginatedItemsViewModel get_application_rounds(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter, school_year=school_year, code=code)

Searches the tenant's application rounds. Default order is school year descending, then code;  `orderBy` accepts `schoolYear` or `code`. Each round carries its windows and  the state of each, derived at the moment of the read.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_application_round_response_dto_paginated_items_view_model import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundResponseDtoPaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.EnrollmentAdminApplicationRoundsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 50 # int |  (optional) (default to 50)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')
    school_year = '' # str | Exact match, e.g. 2026-2027. (optional) (default to '')
    code = '' # str | Exact match. (optional) (default to '')

    try:
        # Searches the tenant's application rounds. Default order is school year descending, then code;  `orderBy` accepts `schoolYear` or `code`. Each round carries its windows and  the state of each, derived at the moment of the read.
        api_response = await api_instance.get_application_rounds(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter, school_year=school_year, code=code)
        print("The response of EnrollmentAdminApplicationRoundsApi->get_application_rounds:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminApplicationRoundsApi->get_application_rounds: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 50]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]
 **school_year** | **str**| Exact match, e.g. 2026-2027. | [optional] [default to &#39;&#39;]
 **code** | **str**| Exact match. | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundResponseDtoPaginatedItemsViewModel**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundResponseDtoPaginatedItemsViewModel.md)

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

# **purge_application_round**
> purge_application_round(tenant_id, id)

Hard-deletes a round. Only a round that has been deleted first.

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
    api_instance = edgraph_platform_client.EnrollmentAdminApplicationRoundsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Hard-deletes a round. Only a round that has been deleted first.
        await api_instance.purge_application_round(tenant_id, id)
    except Exception as e:
        print("Exception when calling EnrollmentAdminApplicationRoundsApi->purge_application_round: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 

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
**204** | The round was purged. |  -  |
**404** | The resource could not be found. |  -  |
**412** | The round has not been deleted. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **recover_application_round**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundMutationResultDto recover_application_round(tenant_id, id)

Brings back a soft-deleted round.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_application_round_mutation_result_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundMutationResultDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminApplicationRoundsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Brings back a soft-deleted round.
        api_response = await api_instance.recover_application_round(tenant_id, id)
        print("The response of EnrollmentAdminApplicationRoundsApi->recover_application_round:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminApplicationRoundsApi->recover_application_round: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundMutationResultDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundMutationResultDto.md)

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
**200** | The round was recovered. |  -  |
**404** | The resource could not be found. |  -  |
**409** | A live round already has this code in this school year. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **remove_application_round_window**
> remove_application_round_window(tenant_id, id, window_id)

Removes one window of the round. Refused while another window depends on it, and when it is  the last window of a round that has opened.

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
    api_instance = edgraph_platform_client.EnrollmentAdminApplicationRoundsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    window_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Removes one window of the round. Refused while another window depends on it, and when it is  the last window of a round that has opened.
        await api_instance.remove_application_round_window(tenant_id, id, window_id)
    except Exception as e:
        print("Exception when calling EnrollmentAdminApplicationRoundsApi->remove_application_round_window: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 
 **window_id** | **UUID**|  | 

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
**204** | The window was removed. |  -  |
**404** | The round or the window could not be found. |  -  |
**412** | Another window depends on it, or it is the last window of an opened round. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_application_round**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundMutationResultDto update_application_round(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_application_round_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_application_round_request_dto)

Replaces a round's label, grades and program types. Code and school year never change -  duplicate the round into another school year instead.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_application_round_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateApplicationRoundRequestDto
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_application_round_mutation_result_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundMutationResultDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminApplicationRoundsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_application_round_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateApplicationRoundRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateApplicationRoundRequestDto |  (optional)

    try:
        # Replaces a round's label, grades and program types. Code and school year never change -  duplicate the round into another school year instead.
        api_response = await api_instance.update_application_round(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_application_round_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_application_round_request_dto)
        print("The response of EnrollmentAdminApplicationRoundsApi->update_application_round:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminApplicationRoundsApi->update_application_round: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_application_round_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateApplicationRoundRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateApplicationRoundRequestDto.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundMutationResultDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundMutationResultDto.md)

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
**200** | The round was updated. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_application_round_window**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundWindowMutationResultDto update_application_round_window(tenant_id, id, window_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto)

Replaces one window of the round.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminEnrollmentWindowRequestDto
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_application_round_window_mutation_result_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundWindowMutationResultDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminApplicationRoundsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    window_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminEnrollmentWindowRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminEnrollmentWindowRequestDto |  (optional)

    try:
        # Replaces one window of the round.
        api_response = await api_instance.update_application_round_window(tenant_id, id, window_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto)
        print("The response of EnrollmentAdminApplicationRoundsApi->update_application_round_window:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminApplicationRoundsApi->update_application_round_window: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 
 **window_id** | **UUID**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminEnrollmentWindowRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminEnrollmentWindowRequestDto.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundWindowMutationResultDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminApplicationRoundWindowMutationResultDto.md)

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
**200** | The window was updated. |  -  |
**400** | Bad Request. The window was invalid, or its dependency names a window that does not exist. |  -  |
**404** | The round or the window could not be found. |  -  |
**412** | The dependency would make windows wait on each other in a loop. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

