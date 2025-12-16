# EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenant


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**status** | [**EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesTenantStatus**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesTenantStatus.md) |  | [optional] 
**roles** | **List[str]** |  | [optional] 
**licenses** | [**List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenantLicense]**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenantLicense.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_tenant import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenant

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenant from a JSON string
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_tenant_instance = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenant.from_json(json)
# print the JSON string representation of the object
print(EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenant.to_json())

# convert the object into a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_tenant_dict = ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_tenant_instance.to_dict()
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenant from a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_tenant_from_dict = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenant.from_dict(ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_tenant_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


