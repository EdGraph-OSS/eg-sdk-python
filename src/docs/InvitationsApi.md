# edgraph_platform_client.InvitationsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_tenant_invitation_async**](InvitationsApi.md#delete_tenant_invitation_async) | **DELETE** /tenants/{tenantId}/invitations/{invitationId} | Deletes an invitation
[**get_all_tenant_invitations_async**](InvitationsApi.md#get_all_tenant_invitations_async) | **GET** /tenants/{tenantId}/invitations | Retrieves a list of invitations associated to this tenant
[**get_tenant_invitation_by_id_async**](InvitationsApi.md#get_tenant_invitation_by_id_async) | **GET** /tenants/{tenantId}/invitations/{invitationId} | Retrieves a specific invitation
[**send_tenant_invitation_async**](InvitationsApi.md#send_tenant_invitation_async) | **POST** /tenants/{tenantId}/invitations | Creates and sends an invitation to a user


# **delete_tenant_invitation_async**
> delete_tenant_invitation_async(tenant_id, invitation_id)

Deletes an invitation

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
with edgraph_platform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = edgraph_platform_client.InvitationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    invitation_id = 'invitation_id_example' # str | 

    try:
        # Deletes an invitation
        api_instance.delete_tenant_invitation_async(tenant_id, invitation_id)
    except Exception as e:
        print("Exception when calling InvitationsApi->delete_tenant_invitation_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **invitation_id** | **str**|  | 

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
**401** | Unauthorized. The request requires authentication. The OAuth bearer token was either not provided or is invalid. The operation may succeed once authentication has been successfully completed. |  -  |
**403** | Forbidden. The request cannot be completed in the current authorization context. Contact your administrator if you believe this operation should be allowed. |  -  |
**500** | An unhandled error occurred on the server.See the response body for details. |  -  |
**204** | The resource was successfully deleted. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_all_tenant_invitations_async**
> IdentityApiInvitationV1InvitationListResponsePaginatedItemsViewModel get_all_tenant_invitations_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves a list of invitations associated to this tenant

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_invitation_v1_invitation_list_response_paginated_items_view_model import IdentityApiInvitationV1InvitationListResponsePaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.InvitationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves a list of invitations associated to this tenant
        api_response = api_instance.get_all_tenant_invitations_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of InvitationsApi->get_all_tenant_invitations_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvitationsApi->get_all_tenant_invitations_async: %s\n" % e)
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

[**IdentityApiInvitationV1InvitationListResponsePaginatedItemsViewModel**](IdentityApiInvitationV1InvitationListResponsePaginatedItemsViewModel.md)

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

# **get_tenant_invitation_by_id_async**
> IdentityApiInvitationV1InvitationResponse get_tenant_invitation_by_id_async(tenant_id, invitation_id)

Retrieves a specific invitation

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.identity_api_invitation_v1_invitation_response import IdentityApiInvitationV1InvitationResponse
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
    api_instance = edgraph_platform_client.InvitationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    invitation_id = 'invitation_id_example' # str | 

    try:
        # Retrieves a specific invitation
        api_response = api_instance.get_tenant_invitation_by_id_async(tenant_id, invitation_id)
        print("The response of InvitationsApi->get_tenant_invitation_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvitationsApi->get_tenant_invitation_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **invitation_id** | **str**|  | 

### Return type

[**IdentityApiInvitationV1InvitationResponse**](IdentityApiInvitationV1InvitationResponse.md)

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

# **send_tenant_invitation_async**
> IdentityApiInvitationV1InvitationSentResponse send_tenant_invitation_async(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_send_invitation_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_send_invitation_request)

Creates and sends an invitation to a user

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_send_invitation_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsSendInvitationRequest
from edgraph_platform_client.models.identity_api_invitation_v1_invitation_sent_response import IdentityApiInvitationV1InvitationSentResponse
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
    api_instance = edgraph_platform_client.InvitationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_send_invitation_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsSendInvitationRequest() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsSendInvitationRequest |  (optional)

    try:
        # Creates and sends an invitation to a user
        api_response = api_instance.send_tenant_invitation_async(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_send_invitation_request=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_send_invitation_request)
        print("The response of InvitationsApi->send_tenant_invitation_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvitationsApi->send_tenant_invitation_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_send_invitation_request** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsSendInvitationRequest**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsSendInvitationRequest.md)|  | [optional] 

### Return type

[**IdentityApiInvitationV1InvitationSentResponse**](IdentityApiInvitationV1InvitationSentResponse.md)

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
**201** | The resource was created. The location of the resource is available in the Location header of the response. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

