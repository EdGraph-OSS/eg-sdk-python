# edgraph_platform_client.InstanceOnboardingStepsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_instance_onboarding_step_async**](InstanceOnboardingStepsApi.md#create_instance_onboarding_step_async) | **POST** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/onboardingsteps | Creates an Onboarding Step.
[**update_instance_onboarding_step_async**](InstanceOnboardingStepsApi.md#update_instance_onboarding_step_async) | **PUT** /tenants/{tenantId}/edfiadmin/instances/{instanceId}/onboardingsteps/{stepNumber} | Updates the status of an Onboarding Step.


# **create_instance_onboarding_step_async**
> EdfiAdminApiEdfiAdminV1InstanceUpdatedResponse create_instance_onboarding_step_async(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_create_onboarding_step_request=edfi_admin_api_edfi_admin_v1_create_onboarding_step_request)

Creates an Onboarding Step.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_onboarding_step_request import EdfiAdminApiEdfiAdminV1CreateOnboardingStepRequest
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_updated_response import EdfiAdminApiEdfiAdminV1InstanceUpdatedResponse
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
    api_instance = edgraph_platform_client.InstanceOnboardingStepsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    edfi_admin_api_edfi_admin_v1_create_onboarding_step_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1CreateOnboardingStepRequest() # EdfiAdminApiEdfiAdminV1CreateOnboardingStepRequest |  (optional)

    try:
        # Creates an Onboarding Step.
        api_response = await api_instance.create_instance_onboarding_step_async(tenant_id, instance_id, edfi_admin_api_edfi_admin_v1_create_onboarding_step_request=edfi_admin_api_edfi_admin_v1_create_onboarding_step_request)
        print("The response of InstanceOnboardingStepsApi->create_instance_onboarding_step_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstanceOnboardingStepsApi->create_instance_onboarding_step_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **edfi_admin_api_edfi_admin_v1_create_onboarding_step_request** | [**EdfiAdminApiEdfiAdminV1CreateOnboardingStepRequest**](EdfiAdminApiEdfiAdminV1CreateOnboardingStepRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1InstanceUpdatedResponse**](EdfiAdminApiEdfiAdminV1InstanceUpdatedResponse.md)

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

# **update_instance_onboarding_step_async**
> EdfiAdminApiEdfiAdminV1InstanceUpdatedResponse update_instance_onboarding_step_async(tenant_id, instance_id, step_number, edfi_admin_api_edfi_admin_v1_update_onboarding_step_request=edfi_admin_api_edfi_admin_v1_update_onboarding_step_request)

Updates the status of an Onboarding Step.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_updated_response import EdfiAdminApiEdfiAdminV1InstanceUpdatedResponse
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_onboarding_step_request import EdfiAdminApiEdfiAdminV1UpdateOnboardingStepRequest
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
    api_instance = edgraph_platform_client.InstanceOnboardingStepsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    step_number = 56 # int | 
    edfi_admin_api_edfi_admin_v1_update_onboarding_step_request = edgraph_platform_client.EdfiAdminApiEdfiAdminV1UpdateOnboardingStepRequest() # EdfiAdminApiEdfiAdminV1UpdateOnboardingStepRequest |  (optional)

    try:
        # Updates the status of an Onboarding Step.
        api_response = await api_instance.update_instance_onboarding_step_async(tenant_id, instance_id, step_number, edfi_admin_api_edfi_admin_v1_update_onboarding_step_request=edfi_admin_api_edfi_admin_v1_update_onboarding_step_request)
        print("The response of InstanceOnboardingStepsApi->update_instance_onboarding_step_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstanceOnboardingStepsApi->update_instance_onboarding_step_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **step_number** | **int**|  | 
 **edfi_admin_api_edfi_admin_v1_update_onboarding_step_request** | [**EdfiAdminApiEdfiAdminV1UpdateOnboardingStepRequest**](EdfiAdminApiEdfiAdminV1UpdateOnboardingStepRequest.md)|  | [optional] 

### Return type

[**EdfiAdminApiEdfiAdminV1InstanceUpdatedResponse**](EdfiAdminApiEdfiAdminV1InstanceUpdatedResponse.md)

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

