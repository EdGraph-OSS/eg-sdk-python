# edgraph_platform_client.RegistrationsAzureMarketplaceApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**submit_tenant_registration_azure_mona_async**](RegistrationsAzureMarketplaceApi.md#submit_tenant_registration_azure_mona_async) | **POST** /registrations/azure/mona | Submits a tenant&#39;s registration request received through Azure [M]arketplace [On]boarding [A]ccelerator (MONA)


# **submit_tenant_registration_azure_mona_async**
> str submit_tenant_registration_azure_mona_async(registration_api_registration_v2_submit_tenant_registration_request=registration_api_registration_v2_submit_tenant_registration_request)

Submits a tenant's registration request received through Azure [M]arketplace [On]boarding [A]ccelerator (MONA)

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.registration_api_registration_v2_submit_tenant_registration_request import RegistrationApiRegistrationV2SubmitTenantRegistrationRequest
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
    api_instance = edgraph_platform_client.RegistrationsAzureMarketplaceApi(api_client)
    registration_api_registration_v2_submit_tenant_registration_request = edgraph_platform_client.RegistrationApiRegistrationV2SubmitTenantRegistrationRequest() # RegistrationApiRegistrationV2SubmitTenantRegistrationRequest |  (optional)

    try:
        # Submits a tenant's registration request received through Azure [M]arketplace [On]boarding [A]ccelerator (MONA)
        api_response = await api_instance.submit_tenant_registration_azure_mona_async(registration_api_registration_v2_submit_tenant_registration_request=registration_api_registration_v2_submit_tenant_registration_request)
        print("The response of RegistrationsAzureMarketplaceApi->submit_tenant_registration_azure_mona_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RegistrationsAzureMarketplaceApi->submit_tenant_registration_azure_mona_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registration_api_registration_v2_submit_tenant_registration_request** | [**RegistrationApiRegistrationV2SubmitTenantRegistrationRequest**](RegistrationApiRegistrationV2SubmitTenantRegistrationRequest.md)|  | [optional] 

### Return type

**str**

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

