# edgraph_platform_client.EnvironmentsReportingPeriodsCategoriesApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search_state_reporting_period_categories**](EnvironmentsReportingPeriodsCategoriesApi.md#search_state_reporting_period_categories) | **GET** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/categories | Retrieves the Categories of a Reporting Period.
[**search_state_reporting_period_sub_categories**](EnvironmentsReportingPeriodsCategoriesApi.md#search_state_reporting_period_sub_categories) | **GET** /tenants/{tenantId}/statereporting/environments/{environmentId}/reportingperiods/{reportingPeriodId}/categories/{categoryId}/subcategories | Retrieves the Sub-Categories of a Reporting Period.


# **search_state_reporting_period_categories**
> EdGraphServicesStateReportingV1PaginatedCategories search_state_reporting_period_categories(tenant_id, environment_id, reporting_period_id, page_index=page_index, page_size=page_size, order_by=order_by)

Retrieves the Categories of a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_paginated_categories import EdGraphServicesStateReportingV1PaginatedCategories
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsCategoriesApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    reporting_period_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_index = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    order_by = 'order_by_example' # str |  (optional)

    try:
        # Retrieves the Categories of a Reporting Period.
        api_response = await api_instance.search_state_reporting_period_categories(tenant_id, environment_id, reporting_period_id, page_index=page_index, page_size=page_size, order_by=order_by)
        print("The response of EnvironmentsReportingPeriodsCategoriesApi->search_state_reporting_period_categories:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsCategoriesApi->search_state_reporting_period_categories: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **reporting_period_id** | **UUID**|  | 
 **page_index** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **order_by** | **str**|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1PaginatedCategories**](EdGraphServicesStateReportingV1PaginatedCategories.md)

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

# **search_state_reporting_period_sub_categories**
> EdGraphServicesStateReportingV1PaginatedSubCategories search_state_reporting_period_sub_categories(tenant_id, environment_id, reporting_period_id, category_id, page_index=page_index, page_size=page_size, order_by=order_by)

Retrieves the Sub-Categories of a Reporting Period.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_paginated_sub_categories import EdGraphServicesStateReportingV1PaginatedSubCategories
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
    api_instance = edgraph_platform_client.EnvironmentsReportingPeriodsCategoriesApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    environment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    reporting_period_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    category_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_index = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    order_by = 'order_by_example' # str |  (optional)

    try:
        # Retrieves the Sub-Categories of a Reporting Period.
        api_response = await api_instance.search_state_reporting_period_sub_categories(tenant_id, environment_id, reporting_period_id, category_id, page_index=page_index, page_size=page_size, order_by=order_by)
        print("The response of EnvironmentsReportingPeriodsCategoriesApi->search_state_reporting_period_sub_categories:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnvironmentsReportingPeriodsCategoriesApi->search_state_reporting_period_sub_categories: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **environment_id** | **UUID**|  | 
 **reporting_period_id** | **UUID**|  | 
 **category_id** | **UUID**|  | 
 **page_index** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **order_by** | **str**|  | [optional] 

### Return type

[**EdGraphServicesStateReportingV1PaginatedSubCategories**](EdGraphServicesStateReportingV1PaginatedSubCategories.md)

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

