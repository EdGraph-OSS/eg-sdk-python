# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsUpdateTenantRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**additional_settings** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsTenantAdditionalSetting**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsTenantAdditionalSetting.md) |  | [optional] 
**identity_providers** | [**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsTenantIdentityProviders]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsTenantIdentityProviders.md) |  | [optional] 
**settings** | [**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsTenantSetting]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsTenantSetting.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_update_tenant_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsUpdateTenantRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsUpdateTenantRequest from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_update_tenant_request_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsUpdateTenantRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsUpdateTenantRequest.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_update_tenant_request_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_update_tenant_request_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsUpdateTenantRequest from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_update_tenant_request_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsTenantsUpdateTenantRequest.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_tenants_update_tenant_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


