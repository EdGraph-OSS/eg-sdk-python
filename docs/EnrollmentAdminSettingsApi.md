# edgraph_platform_client.EnrollmentAdminSettingsApi

All URIs are relative to *https://api.dev.edgraph.com/tenant*

Method | HTTP request | Description
------------- | ------------- | -------------
[**publish_enrollment_settings**](EnrollmentAdminSettingsApi.md#publish_enrollment_settings) | **POST** /tenants/{tenantId}/enrollmentadmin/settings/publish | Publishes the tenant&#39;s current enrollment settings (custom branding, global configuration,  policy acknowledgement URLs) to the public enrollment site.


# **publish_enrollment_settings**
> EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminPublishEnrollmentSettingsResultDto publish_enrollment_settings(tenant_id)

Publishes the tenant's current enrollment settings (custom branding, global configuration,  policy acknowledgement URLs) to the public enrollment site.

### Example

* OAuth Authentication (oauth2):

```python
import edgraph_platform_client
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_publish_enrollment_settings_result_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminPublishEnrollmentSettingsResultDto
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
    api_instance = edgraph_platform_client.EnrollmentAdminSettingsApi(api_client)
    tenant_id = 'tenant_id_example' # str | 

    try:
        # Publishes the tenant's current enrollment settings (custom branding, global configuration,  policy acknowledgement URLs) to the public enrollment site.
        api_response = await api_instance.publish_enrollment_settings(tenant_id)
        print("The response of EnrollmentAdminSettingsApi->publish_enrollment_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnrollmentAdminSettingsApi->publish_enrollment_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_id** | **str**|  | 

### Return type

[**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminPublishEnrollmentSettingsResultDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminPublishEnrollmentSettingsResultDto.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |
**500** | Server Error |  -  |
**200** | The requested resource was successfully retrieved. |  -  |
**400** | Bad Request. The request was invalid and cannot be completed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

