# edgraph_platform_client.AnalyticsDataLakeApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_paginated_lakehouse_records**](AnalyticsDataLakeApi.md#get_paginated_lakehouse_records) | **GET** /tenants/{tenantId}/analytics/datalake/query | Retrieves gold-tier data from the lakehouse


# **get_paginated_lakehouse_records**
> AnalyticsApiLakehousesV1PaginatedLakehouseRecordsResponse get_paginated_lakehouse_records(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves gold-tier data from the lakehouse

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_lakehouses_v1_paginated_lakehouse_records_response import AnalyticsApiLakehousesV1PaginatedLakehouseRecordsResponse
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
    api_instance = edgraph_platform_client.AnalyticsDataLakeApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves gold-tier data from the lakehouse
        api_response = await api_instance.get_paginated_lakehouse_records(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of AnalyticsDataLakeApi->get_paginated_lakehouse_records:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnalyticsDataLakeApi->get_paginated_lakehouse_records: %s\n" % e)
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

[**AnalyticsApiLakehousesV1PaginatedLakehouseRecordsResponse**](AnalyticsApiLakehousesV1PaginatedLakehouseRecordsResponse.md)

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

