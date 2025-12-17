# edgraph_platform_client.ClientsSecretsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_client_secret**](ClientsSecretsApi.md#add_client_secret) | **POST** /tenants/{tenantId}/oneroster/instances/{instanceId}/clients/{clientId}/secrets | Creates a new secret for an OpenId client
[**regenerate_one_roster_api_client_secret_async**](ClientsSecretsApi.md#regenerate_one_roster_api_client_secret_async) | **PUT** /tenants/{tenantId}/oneroster/instances/{instanceId}/clients/{clientId}/regeneratesecret | Regenerate Client Secret


# **add_client_secret**
> IMSAdminApiV1ClientsClientSecretAddedResponse add_client_secret(tenant_id, instance_id, client_id, ims_admin_api_v1_clients_add_client_secret_request=ims_admin_api_v1_clients_add_client_secret_request)

Creates a new secret for an OpenId client

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_clients_add_client_secret_request import IMSAdminApiV1ClientsAddClientSecretRequest
from edgraph_platform_client.models.ims_admin_api_v1_clients_client_secret_added_response import IMSAdminApiV1ClientsClientSecretAddedResponse
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
    api_instance = edgraph_platform_client.ClientsSecretsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    client_id = 'client_id_example' # str | 
    ims_admin_api_v1_clients_add_client_secret_request = edgraph_platform_client.IMSAdminApiV1ClientsAddClientSecretRequest() # IMSAdminApiV1ClientsAddClientSecretRequest |  (optional)

    try:
        # Creates a new secret for an OpenId client
        api_response = api_instance.add_client_secret(tenant_id, instance_id, client_id, ims_admin_api_v1_clients_add_client_secret_request=ims_admin_api_v1_clients_add_client_secret_request)
        print("The response of ClientsSecretsApi->add_client_secret:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ClientsSecretsApi->add_client_secret: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **client_id** | **str**|  | 
 **ims_admin_api_v1_clients_add_client_secret_request** | [**IMSAdminApiV1ClientsAddClientSecretRequest**](IMSAdminApiV1ClientsAddClientSecretRequest.md)|  | [optional] 

### Return type

[**IMSAdminApiV1ClientsClientSecretAddedResponse**](IMSAdminApiV1ClientsClientSecretAddedResponse.md)

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

# **regenerate_one_roster_api_client_secret_async**
> IMSAdminApiV1ClientsClientSecretRegeneratedResponse regenerate_one_roster_api_client_secret_async(tenant_id, instance_id, client_id, ims_admin_api_v1_clients_regenerate_client_secret_request=ims_admin_api_v1_clients_regenerate_client_secret_request)

Regenerate Client Secret

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ims_admin_api_v1_clients_client_secret_regenerated_response import IMSAdminApiV1ClientsClientSecretRegeneratedResponse
from edgraph_platform_client.models.ims_admin_api_v1_clients_regenerate_client_secret_request import IMSAdminApiV1ClientsRegenerateClientSecretRequest
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
    api_instance = edgraph_platform_client.ClientsSecretsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 
    instance_id = 'instance_id_example' # str | 
    client_id = 'client_id_example' # str | 
    ims_admin_api_v1_clients_regenerate_client_secret_request = edgraph_platform_client.IMSAdminApiV1ClientsRegenerateClientSecretRequest() # IMSAdminApiV1ClientsRegenerateClientSecretRequest |  (optional)

    try:
        # Regenerate Client Secret
        api_response = api_instance.regenerate_one_roster_api_client_secret_async(tenant_id, instance_id, client_id, ims_admin_api_v1_clients_regenerate_client_secret_request=ims_admin_api_v1_clients_regenerate_client_secret_request)
        print("The response of ClientsSecretsApi->regenerate_one_roster_api_client_secret_async:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ClientsSecretsApi->regenerate_one_roster_api_client_secret_async: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 
 **instance_id** | **str**|  | 
 **client_id** | **str**|  | 
 **ims_admin_api_v1_clients_regenerate_client_secret_request** | [**IMSAdminApiV1ClientsRegenerateClientSecretRequest**](IMSAdminApiV1ClientsRegenerateClientSecretRequest.md)|  | [optional] 

### Return type

[**IMSAdminApiV1ClientsClientSecretRegeneratedResponse**](IMSAdminApiV1ClientsClientSecretRegeneratedResponse.md)

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

