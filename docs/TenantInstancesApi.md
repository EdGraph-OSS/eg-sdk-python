# edgraph_platform_client.TenantInstancesApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**load_onboarding_step_ed_fi_api_metadata**](TenantInstancesApi.md#load_onboarding_step_ed_fi_api_metadata) | **POST** /tenants/{tenantId}/onboardingsteps/edfi-api-metadata | Loads connection metadata.
[**test_onboarding_step_connection**](TenantInstancesApi.md#test_onboarding_step_connection) | **POST** /tenants/{tenantId}/onboardingsteps/testconnection | Tests availability of provided connection metadata.


# **load_onboarding_step_ed_fi_api_metadata**
> EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsEdFiApiLoadEdFiApiMetadataResult load_onboarding_step_ed_fi_api_metadata(tenant_id, ed_graph_http_aggregators_tenant_api_services_onboarding_steps_use_cases_ed_fi_api_metadata_request=ed_graph_http_aggregators_tenant_api_services_onboarding_steps_use_cases_ed_fi_api_metadata_request)

Loads connection metadata.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_onboarding_steps_ed_fi_api_load_ed_fi_api_metadata_result import EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsEdFiApiLoadEdFiApiMetadataResult
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_onboarding_steps_use_cases_ed_fi_api_metadata_request import EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsUseCasesEdFiApiMetadataRequest
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
    api_instance = edgraph_platform_client.TenantInstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    ed_graph_http_aggregators_tenant_api_services_onboarding_steps_use_cases_ed_fi_api_metadata_request = edgraph_platform_client.EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsUseCasesEdFiApiMetadataRequest() # EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsUseCasesEdFiApiMetadataRequest |  (optional)

    try:
        # Loads connection metadata.
        api_response = await api_instance.load_onboarding_step_ed_fi_api_metadata(tenant_id, ed_graph_http_aggregators_tenant_api_services_onboarding_steps_use_cases_ed_fi_api_metadata_request=ed_graph_http_aggregators_tenant_api_services_onboarding_steps_use_cases_ed_fi_api_metadata_request)
        print("The response of TenantInstancesApi->load_onboarding_step_ed_fi_api_metadata:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantInstancesApi->load_onboarding_step_ed_fi_api_metadata: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **ed_graph_http_aggregators_tenant_api_services_onboarding_steps_use_cases_ed_fi_api_metadata_request** | [**EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsUseCasesEdFiApiMetadataRequest**](EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsUseCasesEdFiApiMetadataRequest.md)|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsEdFiApiLoadEdFiApiMetadataResult**](EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsEdFiApiLoadEdFiApiMetadataResult.md)

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

# **test_onboarding_step_connection**
> EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsTestConnectionResponse test_onboarding_step_connection(tenant_id, body=body)

Tests availability of provided connection metadata.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_onboarding_steps_test_connection_response import EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsTestConnectionResponse
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
    api_instance = edgraph_platform_client.TenantInstancesApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    body = None # object |  (optional)

    try:
        # Tests availability of provided connection metadata.
        api_response = await api_instance.test_onboarding_step_connection(tenant_id, body=body)
        print("The response of TenantInstancesApi->test_onboarding_step_connection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantInstancesApi->test_onboarding_step_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **body** | **object**|  | [optional] 

### Return type

[**EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsTestConnectionResponse**](EdGraphHttpAggregatorsTenantApiServicesOnboardingStepsTestConnectionResponse.md)

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

