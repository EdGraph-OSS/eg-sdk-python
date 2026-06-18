# edgraph_platform_client.ConfigurationsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_analytics_configuration_async**](ConfigurationsApi.md#create_analytics_configuration_async) | **POST** /tenants/{tenantId}/analytics/configurations | Creates a new configuration.
[**delete_analytics_configuration_async**](ConfigurationsApi.md#delete_analytics_configuration_async) | **DELETE** /tenants/{tenantId}/analytics/configurations/{configurationId} | Deletes a configuration.
[**get_all_analytics_configurations_async**](ConfigurationsApi.md#get_all_analytics_configurations_async) | **GET** /tenants/{tenantId}/analytics/configurations | Retrieves all configurations.
[**get_analytics_configuration_by_id_async**](ConfigurationsApi.md#get_analytics_configuration_by_id_async) | **GET** /tenants/{tenantId}/analytics/configurations/{configurationId} | Retrieves a configuration by ID.
[**get_analytics_configuration_by_tenant_id_async**](ConfigurationsApi.md#get_analytics_configuration_by_tenant_id_async) | **GET** /tenants/{tenantId}/analytics/configurations/default | Retrieves current default configuration.
[**has_valid_analytics_configuration_async**](ConfigurationsApi.md#has_valid_analytics_configuration_async) | **GET** /tenants/{tenantId}/analytics/configurations/default/valid | Verifies if current default configuration has required values for correct functionality.
[**update_analytics_configuration_async**](ConfigurationsApi.md#update_analytics_configuration_async) | **PUT** /tenants/{tenantId}/analytics/configurations/{configurationId} | Updates a configuration.
[**validate_aad_token_async**](ConfigurationsApi.md#validate_aad_token_async) | **POST** /tenants/{tenantId}/analytics/configurations/azure/testconnection | Verifies if AAD token generation is possible with user provided values.


# **create_analytics_configuration_async**
> AnalyticsApiConfigurationsV1AnalyticsConfiguration create_analytics_configuration_async(tenant_id, workspace_name, analytics_api_configurations_v1_create_configuration_request=analytics_api_configurations_v1_create_configuration_request)

Creates a new configuration.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_configurations_v1_analytics_configuration import AnalyticsApiConfigurationsV1AnalyticsConfiguration
from edgraph_platform_client.models.analytics_api_configurations_v1_create_configuration_request import AnalyticsApiConfigurationsV1CreateConfigurationRequest
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
    api_instance = edgraph_platform_client.ConfigurationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    workspace_name = 'workspace_name_example' # str | 
    analytics_api_configurations_v1_create_configuration_request = edgraph_platform_client.AnalyticsApiConfigurationsV1CreateConfigurationRequest() # AnalyticsApiConfigurationsV1CreateConfigurationRequest |  (optional)

    try:
        # Creates a new configuration.
        api_response = await api_instance.create_analytics_configuration_async(tenant_id, workspace_name, analytics_api_configurations_v1_create_configuration_request=analytics_api_configurations_v1_create_configuration_request)
        print("The response of ConfigurationsApi->create_analytics_configuration_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConfigurationsApi->create_analytics_configuration_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **workspace_name** | **str**|  | 
 **analytics_api_configurations_v1_create_configuration_request** | [**AnalyticsApiConfigurationsV1CreateConfigurationRequest**](AnalyticsApiConfigurationsV1CreateConfigurationRequest.md)|  | [optional] 

### Return type

[**AnalyticsApiConfigurationsV1AnalyticsConfiguration**](AnalyticsApiConfigurationsV1AnalyticsConfiguration.md)

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
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_analytics_configuration_async**
> delete_analytics_configuration_async(tenant_id, configuration_id)

Deletes a configuration.

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
    api_instance = edgraph_platform_client.ConfigurationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    configuration_id = 'configuration_id_example' # str | 

    try:
        # Deletes a configuration.
        await api_instance.delete_analytics_configuration_async(tenant_id, configuration_id)
    except Exception as e:
        print("Exception when calling ConfigurationsApi->delete_analytics_configuration_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **configuration_id** | **str**|  | 

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
**200** | The requested resource was successfully retrieved. |  -  |
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_all_analytics_configurations_async**
> AnalyticsApiConfigurationsV1AnalyticsConfigurationPaginatedItemsViewModel get_all_analytics_configurations_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)

Retrieves all configurations.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_configurations_v1_analytics_configuration_paginated_items_view_model import AnalyticsApiConfigurationsV1AnalyticsConfigurationPaginatedItemsViewModel
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
    api_instance = edgraph_platform_client.ConfigurationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    page_size = 10 # int |  (optional) (default to 10)
    page_index = 0 # int |  (optional) (default to 0)
    order_by = '' # str |  (optional) (default to '')
    filter = '' # str |  (optional) (default to '')

    try:
        # Retrieves all configurations.
        api_response = await api_instance.get_all_analytics_configurations_async(tenant_id, page_size=page_size, page_index=page_index, order_by=order_by, filter=filter)
        print("The response of ConfigurationsApi->get_all_analytics_configurations_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConfigurationsApi->get_all_analytics_configurations_async: %s\n" % e)
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

[**AnalyticsApiConfigurationsV1AnalyticsConfigurationPaginatedItemsViewModel**](AnalyticsApiConfigurationsV1AnalyticsConfigurationPaginatedItemsViewModel.md)

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

# **get_analytics_configuration_by_id_async**
> AnalyticsApiConfigurationsV1AnalyticsConfiguration get_analytics_configuration_by_id_async(tenant_id, configuration_id)

Retrieves a configuration by ID.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_configurations_v1_analytics_configuration import AnalyticsApiConfigurationsV1AnalyticsConfiguration
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
    api_instance = edgraph_platform_client.ConfigurationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    configuration_id = 'configuration_id_example' # str | 

    try:
        # Retrieves a configuration by ID.
        api_response = await api_instance.get_analytics_configuration_by_id_async(tenant_id, configuration_id)
        print("The response of ConfigurationsApi->get_analytics_configuration_by_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConfigurationsApi->get_analytics_configuration_by_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **configuration_id** | **str**|  | 

### Return type

[**AnalyticsApiConfigurationsV1AnalyticsConfiguration**](AnalyticsApiConfigurationsV1AnalyticsConfiguration.md)

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

# **get_analytics_configuration_by_tenant_id_async**
> AnalyticsApiConfigurationsV1AnalyticsConfiguration get_analytics_configuration_by_tenant_id_async(tenant_id)

Retrieves current default configuration.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_configurations_v1_analytics_configuration import AnalyticsApiConfigurationsV1AnalyticsConfiguration
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
    api_instance = edgraph_platform_client.ConfigurationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 

    try:
        # Retrieves current default configuration.
        api_response = await api_instance.get_analytics_configuration_by_tenant_id_async(tenant_id)
        print("The response of ConfigurationsApi->get_analytics_configuration_by_tenant_id_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConfigurationsApi->get_analytics_configuration_by_tenant_id_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 

### Return type

[**AnalyticsApiConfigurationsV1AnalyticsConfiguration**](AnalyticsApiConfigurationsV1AnalyticsConfiguration.md)

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

# **has_valid_analytics_configuration_async**
> AnalyticsApiConfigurationsV1HasValidConfigurationResponse has_valid_analytics_configuration_async(tenant_id)

Verifies if current default configuration has required values for correct functionality.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_configurations_v1_has_valid_configuration_response import AnalyticsApiConfigurationsV1HasValidConfigurationResponse
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
    api_instance = edgraph_platform_client.ConfigurationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 

    try:
        # Verifies if current default configuration has required values for correct functionality.
        api_response = await api_instance.has_valid_analytics_configuration_async(tenant_id)
        print("The response of ConfigurationsApi->has_valid_analytics_configuration_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConfigurationsApi->has_valid_analytics_configuration_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 

### Return type

[**AnalyticsApiConfigurationsV1HasValidConfigurationResponse**](AnalyticsApiConfigurationsV1HasValidConfigurationResponse.md)

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

# **update_analytics_configuration_async**
> AnalyticsApiConfigurationsV1ConfigurationResponse update_analytics_configuration_async(tenant_id, configuration_id, analytics_api_configurations_v1_update_configuration_request=analytics_api_configurations_v1_update_configuration_request)

Updates a configuration.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_configurations_v1_configuration_response import AnalyticsApiConfigurationsV1ConfigurationResponse
from edgraph_platform_client.models.analytics_api_configurations_v1_update_configuration_request import AnalyticsApiConfigurationsV1UpdateConfigurationRequest
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
    api_instance = edgraph_platform_client.ConfigurationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    configuration_id = 'configuration_id_example' # str | 
    analytics_api_configurations_v1_update_configuration_request = edgraph_platform_client.AnalyticsApiConfigurationsV1UpdateConfigurationRequest() # AnalyticsApiConfigurationsV1UpdateConfigurationRequest |  (optional)

    try:
        # Updates a configuration.
        api_response = await api_instance.update_analytics_configuration_async(tenant_id, configuration_id, analytics_api_configurations_v1_update_configuration_request=analytics_api_configurations_v1_update_configuration_request)
        print("The response of ConfigurationsApi->update_analytics_configuration_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConfigurationsApi->update_analytics_configuration_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **configuration_id** | **str**|  | 
 **analytics_api_configurations_v1_update_configuration_request** | [**AnalyticsApiConfigurationsV1UpdateConfigurationRequest**](AnalyticsApiConfigurationsV1UpdateConfigurationRequest.md)|  | [optional] 

### Return type

[**AnalyticsApiConfigurationsV1ConfigurationResponse**](AnalyticsApiConfigurationsV1ConfigurationResponse.md)

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
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validate_aad_token_async**
> AnalyticsApiConfigurationsV1TestConnectionResponse validate_aad_token_async(tenant_id, analytics_api_configurations_v1_analytics_azure_ad=analytics_api_configurations_v1_analytics_azure_ad)

Verifies if AAD token generation is possible with user provided values.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.analytics_api_configurations_v1_analytics_azure_ad import AnalyticsApiConfigurationsV1AnalyticsAzureAd
from edgraph_platform_client.models.analytics_api_configurations_v1_test_connection_response import AnalyticsApiConfigurationsV1TestConnectionResponse
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
    api_instance = edgraph_platform_client.ConfigurationsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    analytics_api_configurations_v1_analytics_azure_ad = edgraph_platform_client.AnalyticsApiConfigurationsV1AnalyticsAzureAd() # AnalyticsApiConfigurationsV1AnalyticsAzureAd |  (optional)

    try:
        # Verifies if AAD token generation is possible with user provided values.
        api_response = await api_instance.validate_aad_token_async(tenant_id, analytics_api_configurations_v1_analytics_azure_ad=analytics_api_configurations_v1_analytics_azure_ad)
        print("The response of ConfigurationsApi->validate_aad_token_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConfigurationsApi->validate_aad_token_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **analytics_api_configurations_v1_analytics_azure_ad** | [**AnalyticsApiConfigurationsV1AnalyticsAzureAd**](AnalyticsApiConfigurationsV1AnalyticsAzureAd.md)|  | [optional] 

### Return type

[**AnalyticsApiConfigurationsV1TestConnectionResponse**](AnalyticsApiConfigurationsV1TestConnectionResponse.md)

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
**404** | Not Found |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. See the response body for specific validation errors. This will typically be an issue with the query parameters or the request body values. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

