# edgraph_platform_client.AnalyticsConnectorsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_connector**](AnalyticsConnectorsApi.md#create_connector) | **POST** /tenants/{tenantId}/analytics/connectors | Creates a new connector
[**delete_connector**](AnalyticsConnectorsApi.md#delete_connector) | **DELETE** /tenants/{tenantId}/analytics/connectors/{connectorId} | Deletes a connector by Id
[**get_adls_gen2_connector_by_id**](AnalyticsConnectorsApi.md#get_adls_gen2_connector_by_id) | **GET** /tenants/{tenantId}/analytics/connectors/{connectorId} | Retrieves a connector profile by Id
[**get_paginated_connectors**](AnalyticsConnectorsApi.md#get_paginated_connectors) | **GET** /tenants/{tenantId}/analytics/connectors | Retrieves paginated connectors
[**update_connector**](AnalyticsConnectorsApi.md#update_connector) | **PUT** /tenants/{tenantId}/analytics/connectors/{connectorId} | Updates a connector by Id


# **create_connector**
> EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorByTypeCreatedResponse create_connector(tenant_id, body=body)

Creates a new connector

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_connectors_responses_connector_by_type_created_response import EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorByTypeCreatedResponse
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
    api_instance = edgraph_platform_client.AnalyticsConnectorsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    body = None # object |  (optional)

    try:
        # Creates a new connector
        api_response = await api_instance.create_connector(tenant_id, body=body)
        print("The response of AnalyticsConnectorsApi->create_connector:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnalyticsConnectorsApi->create_connector: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **body** | **object**|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorByTypeCreatedResponse**](EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorByTypeCreatedResponse.md)

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
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_connector**
> AnalyticsApiConnectorsV1ConnectorDeletedResponse delete_connector(tenant_id, connector_id)

Deletes a connector by Id

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_connectors_v1_connector_deleted_response import AnalyticsApiConnectorsV1ConnectorDeletedResponse
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
    api_instance = edgraph_platform_client.AnalyticsConnectorsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    connector_id = 'connector_id_example' # str | 

    try:
        # Deletes a connector by Id
        api_response = await api_instance.delete_connector(tenant_id, connector_id)
        print("The response of AnalyticsConnectorsApi->delete_connector:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnalyticsConnectorsApi->delete_connector: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **connector_id** | **str**|  | 

### Return type

[**AnalyticsApiConnectorsV1ConnectorDeletedResponse**](AnalyticsApiConnectorsV1ConnectorDeletedResponse.md)

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

# **get_adls_gen2_connector_by_id**
> EdGraphHttpAggregatorsTenantApiServicesConnectorsExtensionsADLSGen2ConnectorProfileDTO get_adls_gen2_connector_by_id(tenant_id, connector_id)

Retrieves a connector profile by Id

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_connectors_extensions_adls_gen2_connector_profile_dto import EdGraphHttpAggregatorsTenantApiServicesConnectorsExtensionsADLSGen2ConnectorProfileDTO
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
    api_instance = edgraph_platform_client.AnalyticsConnectorsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    connector_id = 'connector_id_example' # str | 

    try:
        # Retrieves a connector profile by Id
        api_response = await api_instance.get_adls_gen2_connector_by_id(tenant_id, connector_id)
        print("The response of AnalyticsConnectorsApi->get_adls_gen2_connector_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnalyticsConnectorsApi->get_adls_gen2_connector_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **connector_id** | **str**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesConnectorsExtensionsADLSGen2ConnectorProfileDTO**](EdGraphHttpAggregatorsTenantApiServicesConnectorsExtensionsADLSGen2ConnectorProfileDTO.md)

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
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_paginated_connectors**
> EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorsPaginatedItemsResponse get_paginated_connectors(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves paginated connectors

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_connectors_responses_connectors_paginated_items_response import EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorsPaginatedItemsResponse
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
    api_instance = edgraph_platform_client.AnalyticsConnectorsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves paginated connectors
        api_response = await api_instance.get_paginated_connectors(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of AnalyticsConnectorsApi->get_paginated_connectors:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnalyticsConnectorsApi->get_paginated_connectors: %s\n" % e)
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

[**EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorsPaginatedItemsResponse**](EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorsPaginatedItemsResponse.md)

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

# **update_connector**
> EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorByTypeUpdatedResponse update_connector(tenant_id, connector_id, body=body)

Updates a connector by Id

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_connectors_responses_connector_by_type_updated_response import EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorByTypeUpdatedResponse
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
    api_instance = edgraph_platform_client.AnalyticsConnectorsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    connector_id = 'connector_id_example' # str | 
    body = None # object |  (optional)

    try:
        # Updates a connector by Id
        api_response = await api_instance.update_connector(tenant_id, connector_id, body=body)
        print("The response of AnalyticsConnectorsApi->update_connector:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnalyticsConnectorsApi->update_connector: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **connector_id** | **str**|  | 
 **body** | **object**|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorByTypeUpdatedResponse**](EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorByTypeUpdatedResponse.md)

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
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

