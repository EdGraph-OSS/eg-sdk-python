# edgraph_platform_client.OnboardingStepsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_onboarding_step**](OnboardingStepsApi.md#create_onboarding_step) | **POST** /tenants/{tenantId}/onboardingsteps | Creates an Onboarding Step.
[**get_onboarding_steps**](OnboardingStepsApi.md#get_onboarding_steps) | **GET** /tenants/{tenantId}/onboardingsteps | Gets a list of Onboarding Steps.
[**update_onboarding_step**](OnboardingStepsApi.md#update_onboarding_step) | **PUT** /tenants/{tenantId}/onboardingsteps/{stepNumber} | Updates the status of an Onboarding Step.


# **create_onboarding_step**
> TenantApiTenantV1TenantUpdatedResponse create_onboarding_step(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_create_onboarding_step_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_create_onboarding_step_request_dto)

Creates an Onboarding Step.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_create_onboarding_step_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsCreateOnboardingStepRequestDto
from edgraph_platform_client.models.tenant_api_tenant_v1_tenant_updated_response import TenantApiTenantV1TenantUpdatedResponse
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
    api_instance = edgraph_platform_client.OnboardingStepsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_create_onboarding_step_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsCreateOnboardingStepRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsCreateOnboardingStepRequestDto |  (optional)

    try:
        # Creates an Onboarding Step.
        api_response = api_instance.create_onboarding_step(tenant_id, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_create_onboarding_step_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_create_onboarding_step_request_dto)
        print("The response of OnboardingStepsApi->create_onboarding_step:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OnboardingStepsApi->create_onboarding_step: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_create_onboarding_step_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsCreateOnboardingStepRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsCreateOnboardingStepRequestDto.md)|  | [optional] 

### Return type

[**TenantApiTenantV1TenantUpdatedResponse**](TenantApiTenantV1TenantUpdatedResponse.md)

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

# **get_onboarding_steps**
> TenantApiTenantV1OnboardingStepsReponse get_onboarding_steps(tenant_id)

Gets a list of Onboarding Steps.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.tenant_api_tenant_v1_onboarding_steps_reponse import TenantApiTenantV1OnboardingStepsReponse
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
    api_instance = edgraph_platform_client.OnboardingStepsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 

    try:
        # Gets a list of Onboarding Steps.
        api_response = api_instance.get_onboarding_steps(tenant_id)
        print("The response of OnboardingStepsApi->get_onboarding_steps:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OnboardingStepsApi->get_onboarding_steps: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 

### Return type

[**TenantApiTenantV1OnboardingStepsReponse**](TenantApiTenantV1OnboardingStepsReponse.md)

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

# **update_onboarding_step**
> TenantApiTenantV1TenantUpdatedResponse update_onboarding_step(tenant_id, step_number, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_update_onboarding_step_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_update_onboarding_step_request_dto)

Updates the status of an Onboarding Step.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_update_onboarding_step_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsUpdateOnboardingStepRequestDto
from edgraph_platform_client.models.tenant_api_tenant_v1_tenant_updated_response import TenantApiTenantV1TenantUpdatedResponse
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
    api_instance = edgraph_platform_client.OnboardingStepsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    step_number = 56 # int | 
    ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_update_onboarding_step_request_dto = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsUpdateOnboardingStepRequestDto() # EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsUpdateOnboardingStepRequestDto |  (optional)

    try:
        # Updates the status of an Onboarding Step.
        api_response = api_instance.update_onboarding_step(tenant_id, step_number, ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_update_onboarding_step_request_dto=ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_update_onboarding_step_request_dto)
        print("The response of OnboardingStepsApi->update_onboarding_step:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OnboardingStepsApi->update_onboarding_step: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **step_number** | **int**|  | 
 **ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_update_onboarding_step_request_dto** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsUpdateOnboardingStepRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsUpdateOnboardingStepRequestDto.md)|  | [optional] 

### Return type

[**TenantApiTenantV1TenantUpdatedResponse**](TenantApiTenantV1TenantUpdatedResponse.md)

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

