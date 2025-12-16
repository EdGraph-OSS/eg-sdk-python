# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsTenantIdentityProviders


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**identity_provider_id** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsTenantIdentityProviderId**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsTenantIdentityProviderId.md) |  | [optional] 
**identity_provider_status** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsTenantIdentityProviderStatus**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsTenantIdentityProviderStatus.md) |  | [optional] 
**enable_mfa** | **bool** |  | [optional] 
**enforce_mfa** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_tenant_identity_providers import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsTenantIdentityProviders

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsTenantIdentityProviders from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_tenant_identity_providers_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsTenantIdentityProviders.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsTenantIdentityProviders.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_tenant_identity_providers_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_tenant_identity_providers_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsTenantIdentityProviders from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_tenant_identity_providers_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsTenantIdentityProviders.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_tenant_identity_providers_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


