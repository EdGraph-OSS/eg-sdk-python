# edgraph_platform_client.EnrollmentAdminProgramsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_program_catalog_entry**](EnrollmentAdminProgramsApi.md#create_program_catalog_entry) | **POST** /tenants/{tenantId}/enrollmentadmin/programs/catalog-entries | Creates a district catalog entry - a program the district defines once, which schools may  then be offered at. No school-identifying field; use POST .../programs/school-programs to  offer it at a school.
[**create_school_program**](EnrollmentAdminProgramsApi.md#create_school_program) | **POST** /tenants/{tenantId}/enrollmentadmin/programs/school-programs | Creates a school program - either adding an existing district catalog entry to a school  (a \&quot;school association\&quot;, when &#x60;programCatalogEntryId&#x60; is set) or creating a brand new  school-specific program (when it is not).
[**delete_program_catalog_entry**](EnrollmentAdminProgramsApi.md#delete_program_catalog_entry) | **DELETE** /tenants/{tenantId}/enrollmentadmin/programs/catalog-entries/{id} | Removes a district catalog entry.
[**delete_school_program**](EnrollmentAdminProgramsApi.md#delete_school_program) | **DELETE** /tenants/{tenantId}/enrollmentadmin/programs/school-programs/{id} | Removes a school program - the API equivalent of \&quot;remove a school association\&quot; when the  row is linked to a catalog entry, or a straightforward delete when it is school-specific.
[**get_program_by_id**](EnrollmentAdminProgramsApi.md#get_program_by_id) | **GET** /tenants/{tenantId}/enrollmentadmin/programs/{id} | Gets a Program by its record id - a district catalog entry or a school-specific program.
[**get_programs**](EnrollmentAdminProgramsApi.md#get_programs) | **GET** /tenants/{tenantId}/enrollmentadmin/programs | Searches Programs - the union of district catalog entries and school-specific programs, in  one list distinguished by each row&#39;s Scope.
[**update_program_catalog_entry**](EnrollmentAdminProgramsApi.md#update_program_catalog_entry) | **PUT** /tenants/{tenantId}/enrollmentadmin/programs/catalog-entries/{id} | Updates a district catalog entry&#39;s own fields.
[**update_school_program**](EnrollmentAdminProgramsApi.md#update_school_program) | **PUT** /tenants/{tenantId}/enrollmentadmin/programs/school-programs/{id} | Updates a school program&#39;s grades/capacity/zone/coordinates, and - only when it is  school-specific - its own Code/Name/ProgramType/EligibilityCriteria/RequiredDocuments.


# **create_program_catalog_entry**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramMutationResultDto create_program_catalog_entry(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_program_catalog_entry_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_program_catalog_entry_request_dto)

Creates a district catalog entry - a program the district defines once, which schools may  then be offered at. No school-identifying field; use POST .../programs/school-programs to  offer it at a school.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_program_catalog_entry_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateProgramCatalogEntryRequestDto
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_program_mutation_result_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramMutationResultDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminProgramsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_program_catalog_entry_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateProgramCatalogEntryRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateProgramCatalogEntryRequestDto |  (optional)

    try:
        # Creates a district catalog entry - a program the district defines once, which schools may  then be offered at. No school-identifying field; use POST .../programs/school-programs to  offer it at a school.
        api_response = await api_instance.create_program_catalog_entry(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_program_catalog_entry_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_program_catalog_entry_request_dto)
        print("The response of EnrollmentAdminProgramsApi->create_program_catalog_entry:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminProgramsApi->create_program_catalog_entry: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_program_catalog_entry_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateProgramCatalogEntryRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateProgramCatalogEntryRequestDto.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramMutationResultDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramMutationResultDto.md)

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
**201** | The catalog entry was created. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_school_program**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramMutationResultDto create_school_program(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_school_program_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_school_program_request_dto)

Creates a school program - either adding an existing district catalog entry to a school  (a \"school association\", when `programCatalogEntryId` is set) or creating a brand new  school-specific program (when it is not).

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_school_program_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateSchoolProgramRequestDto
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_program_mutation_result_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramMutationResultDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminProgramsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_school_program_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateSchoolProgramRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateSchoolProgramRequestDto |  (optional)

    try:
        # Creates a school program - either adding an existing district catalog entry to a school  (a \"school association\", when `programCatalogEntryId` is set) or creating a brand new  school-specific program (when it is not).
        api_response = await api_instance.create_school_program(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_school_program_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_school_program_request_dto)
        print("The response of EnrollmentAdminProgramsApi->create_school_program:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminProgramsApi->create_school_program: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_school_program_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateSchoolProgramRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateSchoolProgramRequestDto.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramMutationResultDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramMutationResultDto.md)

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
**201** | The school program was created. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_program_catalog_entry**
> delete_program_catalog_entry(tenant_id, id)

Removes a district catalog entry.

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
    api_instance = edgraph_platform_client.EnrollmentAdminProgramsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Removes a district catalog entry.
        await api_instance.delete_program_catalog_entry(tenant_id, id)
    except Exception as e:
        print("Exception when calling EnrollmentAdminProgramsApi->delete_program_catalog_entry: %s\n" % e)
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
**204** | The catalog entry was removed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_school_program**
> delete_school_program(tenant_id, id)

Removes a school program - the API equivalent of \"remove a school association\" when the  row is linked to a catalog entry, or a straightforward delete when it is school-specific.

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
    api_instance = edgraph_platform_client.EnrollmentAdminProgramsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Removes a school program - the API equivalent of \"remove a school association\" when the  row is linked to a catalog entry, or a straightforward delete when it is school-specific.
        await api_instance.delete_school_program(tenant_id, id)
    except Exception as e:
        print("Exception when calling EnrollmentAdminProgramsApi->delete_school_program: %s\n" % e)
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
**204** | The school program was removed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_program_by_id**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramDetailDto get_program_by_id(tenant_id, id)

Gets a Program by its record id - a district catalog entry or a school-specific program.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_program_detail_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramDetailDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminProgramsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Gets a Program by its record id - a district catalog entry or a school-specific program.
        api_response = await api_instance.get_program_by_id(tenant_id, id)
        print("The response of EnrollmentAdminProgramsApi->get_program_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminProgramsApi->get_program_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramDetailDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramDetailDto.md)

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

# **get_programs**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramListItemDtoPaginatedItemsViewModel get_programs(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter, search=search, scope=scope, school_code=school_code, program_type=program_type)

Searches Programs - the union of district catalog entries and school-specific programs, in  one list distinguished by each row's Scope.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_program_list_item_dto_paginated_items_view_model import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramListItemDtoPaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.EnrollmentAdminProgramsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 50 # int |  (optional) (default to 50)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')
    search = '' # str | Free-text match on program name/code. (optional) (default to '')
    scope = '' # str | \"DistrictCatalog\", \"SchoolSpecific\", or omitted for all. (optional) (default to '')
    school_code = '' # str | Narrows to programs offered at this school. Not a security boundary. (optional) (default to '')
    program_type = '' # str |  (optional) (default to '')

    try:
        # Searches Programs - the union of district catalog entries and school-specific programs, in  one list distinguished by each row's Scope.
        api_response = await api_instance.get_programs(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter, search=search, scope=scope, school_code=school_code, program_type=program_type)
        print("The response of EnrollmentAdminProgramsApi->get_programs:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminProgramsApi->get_programs: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 50]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]
 **search** | **str**| Free-text match on program name/code. | [optional] [default to &#39;&#39;]
 **scope** | **str**| \&quot;DistrictCatalog\&quot;, \&quot;SchoolSpecific\&quot;, or omitted for all. | [optional] [default to &#39;&#39;]
 **school_code** | **str**| Narrows to programs offered at this school. Not a security boundary. | [optional] [default to &#39;&#39;]
 **program_type** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramListItemDtoPaginatedItemsViewModel**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramListItemDtoPaginatedItemsViewModel.md)

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

# **update_program_catalog_entry**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramMutationResultDto update_program_catalog_entry(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_program_catalog_entry_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_program_catalog_entry_request_dto)

Updates a district catalog entry's own fields.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_program_catalog_entry_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateProgramCatalogEntryRequestDto
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_program_mutation_result_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramMutationResultDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminProgramsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_program_catalog_entry_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateProgramCatalogEntryRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateProgramCatalogEntryRequestDto |  (optional)

    try:
        # Updates a district catalog entry's own fields.
        api_response = await api_instance.update_program_catalog_entry(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_program_catalog_entry_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_program_catalog_entry_request_dto)
        print("The response of EnrollmentAdminProgramsApi->update_program_catalog_entry:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminProgramsApi->update_program_catalog_entry: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_program_catalog_entry_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateProgramCatalogEntryRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateProgramCatalogEntryRequestDto.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramMutationResultDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramMutationResultDto.md)

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
**200** | The catalog entry was updated. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_school_program**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramMutationResultDto update_school_program(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_school_program_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_school_program_request_dto)

Updates a school program's grades/capacity/zone/coordinates, and - only when it is  school-specific - its own Code/Name/ProgramType/EligibilityCriteria/RequiredDocuments.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_school_program_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateSchoolProgramRequestDto
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_program_mutation_result_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramMutationResultDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminProgramsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_school_program_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateSchoolProgramRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateSchoolProgramRequestDto |  (optional)

    try:
        # Updates a school program's grades/capacity/zone/coordinates, and - only when it is  school-specific - its own Code/Name/ProgramType/EligibilityCriteria/RequiredDocuments.
        api_response = await api_instance.update_school_program(tenant_id, id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_school_program_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_school_program_request_dto)
        print("The response of EnrollmentAdminProgramsApi->update_school_program:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminProgramsApi->update_school_program: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **id** | **UUID**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_school_program_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateSchoolProgramRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateSchoolProgramRequestDto.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramMutationResultDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminProgramMutationResultDto.md)

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
**200** | The school program was updated. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

