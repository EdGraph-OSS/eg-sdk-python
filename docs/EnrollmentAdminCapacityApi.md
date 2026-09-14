# edgraph_platform_client.EnrollmentAdminCapacityApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_capacity**](EnrollmentAdminCapacityApi.md#get_capacity) | **GET** /tenants/{tenantId}/enrollmentadmin/schools/{schoolCode}/capacity | Searches Capacity for one school - one row per program x grade x school year.


# **get_capacity**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminCapacityListItemDtoPaginatedItemsViewModel get_capacity(tenant_id, school_code, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter, grade=grade, search=search)

Searches Capacity for one school - one row per program x grade x school year.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_capacity_list_item_dto_paginated_items_view_model import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminCapacityListItemDtoPaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.EnrollmentAdminCapacityApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    school_code = 'school_code_example' # str | Required - a seat count is meaningless without a school.
    page_size = 50 # int |  (optional) (default to 50)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')
    grade = '' # str | Optional exact match. (optional) (default to '')
    search = '' # str | Free-text match on program name/code. (optional) (default to '')

    try:
        # Searches Capacity for one school - one row per program x grade x school year.
        api_response = await api_instance.get_capacity(tenant_id, school_code, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter, grade=grade, search=search)
        print("The response of EnrollmentAdminCapacityApi->get_capacity:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminCapacityApi->get_capacity: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **school_code** | **str**| Required - a seat count is meaningless without a school. | 
 **page_size** | **int**|  | [optional] [default to 50]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]
 **grade** | **str**| Optional exact match. | [optional] [default to &#39;&#39;]
 **search** | **str**| Free-text match on program name/code. | [optional] [default to &#39;&#39;]

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminCapacityListItemDtoPaginatedItemsViewModel**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminCapacityListItemDtoPaginatedItemsViewModel.md)

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

