# edgraph_platform_client.StateReportingStepsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_steps**](StateReportingStepsApi.md#get_steps) | **GET** /tenants/{tenantId}/statereporting/schoolYear/{schoolYear}/steps | Get Steps Status for the tenant.
[**update_step**](StateReportingStepsApi.md#update_step) | **POST** /tenants/{tenantId}/statereporting/schoolYear/{schoolYear}/steps | Update Steps Status for the tenant.


# **get_steps**
> ValidationsApiStateReportingStepsV1GetStateReportingStepsResponse get_steps(tenant_id, school_year)

Get Steps Status for the tenant.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_state_reporting_steps_v1_get_state_reporting_steps_response import ValidationsApiStateReportingStepsV1GetStateReportingStepsResponse
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
    api_instance = edgraph_platform_client.StateReportingStepsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    school_year = 56 # int | 

    try:
        # Get Steps Status for the tenant.
        api_response = api_instance.get_steps(tenant_id, school_year)
        print("The response of StateReportingStepsApi->get_steps:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StateReportingStepsApi->get_steps: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **school_year** | **int**|  | 

### Return type

[**ValidationsApiStateReportingStepsV1GetStateReportingStepsResponse**](ValidationsApiStateReportingStepsV1GetStateReportingStepsResponse.md)

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

# **update_step**
> ValidationsApiStateReportingStepsV1GetStateReportingStepsResponse update_step(tenant_id, school_year, validations_api_state_reporting_steps_v1_update_state_reporting_step_request=validations_api_state_reporting_steps_v1_update_state_reporting_step_request)

Update Steps Status for the tenant.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.validations_api_state_reporting_steps_v1_get_state_reporting_steps_response import ValidationsApiStateReportingStepsV1GetStateReportingStepsResponse
from edgraph_platform_client.models.validations_api_state_reporting_steps_v1_update_state_reporting_step_request import ValidationsApiStateReportingStepsV1UpdateStateReportingStepRequest
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
    api_instance = edgraph_platform_client.StateReportingStepsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    school_year = 56 # int | 
    validations_api_state_reporting_steps_v1_update_state_reporting_step_request = edgraph_platform_client.ValidationsApiStateReportingStepsV1UpdateStateReportingStepRequest() # ValidationsApiStateReportingStepsV1UpdateStateReportingStepRequest |  (optional)

    try:
        # Update Steps Status for the tenant.
        api_response = api_instance.update_step(tenant_id, school_year, validations_api_state_reporting_steps_v1_update_state_reporting_step_request=validations_api_state_reporting_steps_v1_update_state_reporting_step_request)
        print("The response of StateReportingStepsApi->update_step:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StateReportingStepsApi->update_step: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **school_year** | **int**|  | 
 **validations_api_state_reporting_steps_v1_update_state_reporting_step_request** | [**ValidationsApiStateReportingStepsV1UpdateStateReportingStepRequest**](ValidationsApiStateReportingStepsV1UpdateStateReportingStepRequest.md)|  | [optional] 

### Return type

[**ValidationsApiStateReportingStepsV1GetStateReportingStepsResponse**](ValidationsApiStateReportingStepsV1GetStateReportingStepsResponse.md)

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

