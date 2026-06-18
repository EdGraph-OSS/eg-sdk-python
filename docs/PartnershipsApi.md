# edgraph_platform_client.PartnershipsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_all_partnerships**](PartnershipsApi.md#get_all_partnerships) | **GET** /tenants/{tenantId}/partnerships | Retrieves a list of Partnerships.
[**get_partnership_by_id**](PartnershipsApi.md#get_partnership_by_id) | **GET** /tenants/{tenantId}/partnerships/{partnershipId} | Retrieves a Partnership by ID.


# **get_all_partnerships**
> TenantApiPartnershipV1PaginatedItemsResponse get_all_partnerships(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, partner_tenant_id=partner_tenant_id, partnership_type=partnership_type, exclude_soft_deleted=exclude_soft_deleted)

Retrieves a list of Partnerships.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_partnership_v1_paginated_items_response import TenantApiPartnershipV1PaginatedItemsResponse
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
    api_instance = edgraph_platform_client.PartnershipsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    page_index = 0 # int |  (optional) (default to 0)
    page_size = 10 # int |  (optional) (default to 10)
    order_by = 'order_by_example' # str |  (optional)
    partner_tenant_id = 'partner_tenant_id_example' # str |  (optional)
    partnership_type = ['partnership_type_example'] # List[str] |  (optional)
    exclude_soft_deleted = True # bool |  (optional) (default to True)

    try:
        # Retrieves a list of Partnerships.
        api_response = await api_instance.get_all_partnerships(tenant_id, page_index=page_index, page_size=page_size, order_by=order_by, partner_tenant_id=partner_tenant_id, partnership_type=partnership_type, exclude_soft_deleted=exclude_soft_deleted)
        print("The response of PartnershipsApi->get_all_partnerships:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PartnershipsApi->get_all_partnerships: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **page_index** | **int**|  | [optional] [default to 0]
 **page_size** | **int**|  | [optional] [default to 10]
 **order_by** | **str**|  | [optional] 
 **partner_tenant_id** | **str**|  | [optional] 
 **partnership_type** | [**List[str]**](str.md)|  | [optional] 
 **exclude_soft_deleted** | **bool**|  | [optional] [default to True]

### Return type

[**TenantApiPartnershipV1PaginatedItemsResponse**](TenantApiPartnershipV1PaginatedItemsResponse.md)

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

# **get_partnership_by_id**
> TenantApiPartnershipV1PartnershipByIdResponse get_partnership_by_id(tenant_id, partnership_id, exclude_soft_deleted=exclude_soft_deleted)

Retrieves a Partnership by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_partnership_v1_partnership_by_id_response import TenantApiPartnershipV1PartnershipByIdResponse
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
    api_instance = edgraph_platform_client.PartnershipsApi(api_client)
    tenant_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    partnership_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    exclude_soft_deleted = True # bool |  (optional) (default to True)

    try:
        # Retrieves a Partnership by ID.
        api_response = await api_instance.get_partnership_by_id(tenant_id, partnership_id, exclude_soft_deleted=exclude_soft_deleted)
        print("The response of PartnershipsApi->get_partnership_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PartnershipsApi->get_partnership_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **UUID**|  | 
 **partnership_id** | **UUID**|  | 
 **exclude_soft_deleted** | **bool**|  | [optional] [default to True]

### Return type

[**TenantApiPartnershipV1PartnershipByIdResponse**](TenantApiPartnershipV1PartnershipByIdResponse.md)

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

