# EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesClientBrandingResponse

Public, render-only projection of a client's branding (Azure DevOps #17086) returned by the  unauthenticated GET /clients/{clientId}/branding endpoint. Intentionally minimal — it carries only  the fields a sign-in / pre-auth surface needs to render, plus the override flag so the caller can  apply client-vs-tenant precedence itself. It never exposes secrets, storage internals  (blob/container names), or any other client configuration.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  | [optional] 
**brand_name** | **str** |  | [optional] 
**logo_url** | **str** |  | [optional] 
**background_url** | **str** |  | [optional] 
**allow_tenant_to_override** | **bool** | When false, this client&#39;s branding overrides the tenant&#39;s on the sign-in page. | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_client_branding_response import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesClientBrandingResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesClientBrandingResponse from a JSON string
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_client_branding_response_instance = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesClientBrandingResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesClientBrandingResponse.to_json())

# convert the object into a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_client_branding_response_dict = ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_client_branding_response_instance.to_dict()
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesClientBrandingResponse from a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_client_branding_response_from_dict = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesClientBrandingResponse.from_dict(ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_client_branding_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


