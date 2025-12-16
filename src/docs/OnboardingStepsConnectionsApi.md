# edgraph_platform_client.OnboardingStepsConnectionsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_onboarding_step_connection**](OnboardingStepsConnectionsApi.md#create_onboarding_step_connection) | **POST** /tenants/{tenantId}/onboardingsteps/{stepNumber}/connections | Creates an Onboarding Step connection.
[**get_onboarding_step_connection_by_id**](OnboardingStepsConnectionsApi.md#get_onboarding_step_connection_by_id) | **GET** /tenants/{tenantId}/onboardingsteps/{stepNumber}/connections/{connectionId} | Get an Onboarding Step connection by Id
[**update_onboarding_step_connection**](OnboardingStepsConnectionsApi.md#update_onboarding_step_connection) | **PUT** /tenants/{tenantId}/onboardingsteps/{stepNumber}/connections/{connectionId} | Update an Onboarding Step connection by Id


# **create_onboarding_step_connection**
> EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsConnectionCreatedResponse create_onboarding_step_connection(tenant_id, step_number, body=body)

Creates an Onboarding Step connection.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_onboarding_steps_connection_created_response import EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsConnectionCreatedResponse
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
    api_instance = edgraph_platform_client.OnboardingStepsConnectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    step_number = 56 # int | 
    body = None # object |  (optional)

    try:
        # Creates an Onboarding Step connection.
        api_response = api_instance.create_onboarding_step_connection(tenant_id, step_number, body=body)
        print("The response of OnboardingStepsConnectionsApi->create_onboarding_step_connection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OnboardingStepsConnectionsApi->create_onboarding_step_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **step_number** | **int**|  | 
 **body** | **object**|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsConnectionCreatedResponse**](EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsConnectionCreatedResponse.md)

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

# **get_onboarding_step_connection_by_id**
> EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsConnectionResponse get_onboarding_step_connection_by_id(tenant_id, step_number, connection_id)

Get an Onboarding Step connection by Id

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_onboarding_steps_connection_response import EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsConnectionResponse
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
    api_instance = edgraph_platform_client.OnboardingStepsConnectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    step_number = 56 # int | 
    connection_id = 'connection_id_example' # str | 

    try:
        # Get an Onboarding Step connection by Id
        api_response = api_instance.get_onboarding_step_connection_by_id(tenant_id, step_number, connection_id)
        print("The response of OnboardingStepsConnectionsApi->get_onboarding_step_connection_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OnboardingStepsConnectionsApi->get_onboarding_step_connection_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **step_number** | **int**|  | 
 **connection_id** | **str**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsConnectionResponse**](EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsConnectionResponse.md)

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

# **update_onboarding_step_connection**
> EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsConnectionUpdatedResponse update_onboarding_step_connection(tenant_id, step_number, connection_id, body=body)

Update an Onboarding Step connection by Id

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_onboarding_steps_connection_updated_response import EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsConnectionUpdatedResponse
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
    api_instance = edgraph_platform_client.OnboardingStepsConnectionsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    step_number = 56 # int | 
    connection_id = 'connection_id_example' # str | 
    body = None # object |  (optional)

    try:
        # Update an Onboarding Step connection by Id
        api_response = api_instance.update_onboarding_step_connection(tenant_id, step_number, connection_id, body=body)
        print("The response of OnboardingStepsConnectionsApi->update_onboarding_step_connection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OnboardingStepsConnectionsApi->update_onboarding_step_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **step_number** | **int**|  | 
 **connection_id** | **str**|  | 
 **body** | **object**|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsConnectionUpdatedResponse**](EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsConnectionUpdatedResponse.md)

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
**404** | The resource could not be found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

