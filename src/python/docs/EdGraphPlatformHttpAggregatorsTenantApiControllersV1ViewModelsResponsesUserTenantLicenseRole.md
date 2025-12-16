# EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenantLicenseRole


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**role** | **str** |  | [optional] 
**is_implicitly_assigned** | **bool** |  | [optional] 
**status** | **str** | Maps to EdGraph.Platform.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Responses.UserTenantLicenseRoleStatus.&lt;br&gt;&lt;/br&gt;    For more info on deprecation see: Task 9962: Modify implicit license response to prioritize explicit licenses over implicit (part 2) (https://dev.azure.com/edwire/EW.Educate/_workitems/edit/9962)&lt;br&gt;&lt;/br&gt;    Use EdGraph.Platform.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Responses.LicenseSource instead.&lt;br&gt;&lt;/br&gt; | [optional] 
**education_organization_id** | **int** |  | [optional] 
**staff_classification** | **str** |  | [optional] 
**source** | **str** | Maps to EdGraph.Platform.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Responses.LicenseSource.&lt;br&gt;&lt;/br&gt;    For more info see: Task 9962: Modify implicit license response to prioritize explicit licenses over implicit (part 2) (https://dev.azure.com/edwire/EW.Educate/_workitems/edit/9962) | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_tenant_license_role import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenantLicenseRole

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenantLicenseRole from a JSON string
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_tenant_license_role_instance = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenantLicenseRole.from_json(json)
# print the JSON string representation of the object
print(EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenantLicenseRole.to_json())

# convert the object into a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_tenant_license_role_dict = ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_tenant_license_role_instance.to_dict()
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenantLicenseRole from a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_tenant_license_role_from_dict = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenantLicenseRole.from_dict(ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_tenant_license_role_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


