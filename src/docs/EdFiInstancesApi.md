# edgraph_platform_client.EdFiInstancesApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_all_ed_fi_admin_connections_from_analytics_async**](EdFiInstancesApi.md#get_all_ed_fi_admin_connections_from_analytics_async) | **GET** /tenants/{tenantId}/analytics/edfiadmin/connections | Retrieves a list of EdFi Admin connections
[**get_all_ed_fi_admin_instances_from_analytics_async**](EdFiInstancesApi.md#get_all_ed_fi_admin_instances_from_analytics_async) | **GET** /tenants/{tenantId}/analytics/edfiadmin/instances | Retrieves a list of EdFi Admin instances
[**get_ed_fi_admin_instance_by_id_from_analytics_async**](EdFiInstancesApi.md#get_ed_fi_admin_instance_by_id_from_analytics_async) | **GET** /tenants/{tenantId}/analytics/edfiadmin/instances/{instanceId} | Retrieves an Ed-Fi Admin instance by ID.


# **get_all_ed_fi_admin_connections_from_analytics_async**
> AnalyticsApiReportsV1ReportPaginatedItemsResponse get_all_ed_fi_admin_connections_from_analytics_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of EdFi Admin connections

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_reports_v1_report_paginated_items_response import AnalyticsApiReportsV1ReportPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.EdFiInstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of EdFi Admin connections
        api_response = api_instance.get_all_ed_fi_admin_connections_from_analytics_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of EdFiInstancesApi->get_all_ed_fi_admin_connections_from_analytics_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EdFiInstancesApi->get_all_ed_fi_admin_connections_from_analytics_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**AnalyticsApiReportsV1ReportPaginatedItemsResponse**](AnalyticsApiReportsV1ReportPaginatedItemsResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Missing the required permissions to access to this tenant/resource |  -  |
**500** | Oops! Can&#39;t retrieve the list of EdFi Admin connections right now |  -  |
**200** | List of EdFi Admin connections |  -  |
**400** | Tenant has missing/invalid values |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_all_ed_fi_admin_instances_from_analytics_async**
> AnalyticsApiReportsV1ReportPaginatedItemsResponse get_all_ed_fi_admin_instances_from_analytics_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of EdFi Admin instances

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_reports_v1_report_paginated_items_response import AnalyticsApiReportsV1ReportPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.EdFiInstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of EdFi Admin instances
        api_response = api_instance.get_all_ed_fi_admin_instances_from_analytics_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of EdFiInstancesApi->get_all_ed_fi_admin_instances_from_analytics_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EdFiInstancesApi->get_all_ed_fi_admin_instances_from_analytics_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 10]
 **page_index** | **int**|  | [optional] [default to 0]
 **order_by** | **str**|  | [optional] [default to &#39;&#39;]
 **filter** | **str**|  | [optional] [default to &#39;&#39;]

### Return type

[**AnalyticsApiReportsV1ReportPaginatedItemsResponse**](AnalyticsApiReportsV1ReportPaginatedItemsResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Missing the required permissions to access to this tenant/resource |  -  |
**500** | Oops! Can&#39;t retrieve the list of EdFi Admin instances right now |  -  |
**200** | List of EdFi Admin instances |  -  |
**400** | Tenant has missing/invalid values |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_ed_fi_admin_instance_by_id_from_analytics_async**
> EdfiAdminApiEdfiAdminV1Instance get_ed_fi_admin_instance_by_id_from_analytics_async(tenant_id, instance_id)

Retrieves an Ed-Fi Admin instance by ID.

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
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.EdFiInstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 

    try:
        # Retrieves an Ed-Fi Admin instance by ID.
        api_response = api_instance.get_ed_fi_admin_instance_by_id_from_analytics_async(tenant_id, instance_id)
        print("The response of EdFiInstancesApi->get_ed_fi_admin_instance_by_id_from_analytics_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EdFiInstancesApi->get_ed_fi_admin_instance_by_id_from_analytics_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

