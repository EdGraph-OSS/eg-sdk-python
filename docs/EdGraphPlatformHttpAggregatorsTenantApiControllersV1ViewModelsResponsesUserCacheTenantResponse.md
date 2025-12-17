# EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheTenantResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**tenant_type** | **str** |  | [optional] 
**tenant_types** | **List[str]** |  | [optional] 
**organization_identifier** | **str** |  | [optional] 
**organization_name** | **str** |  | [optional] 
**state** | **str** |  | [optional] 
**tenant_status** | **str** |  | [optional] 
**is_demo** | **bool** |  | [optional] 
**education_organizations** | [**List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheTenantEducationOrganizationResponse]**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheTenantEducationOrganizationResponse.md) |  | [optional] 
**licenses** | [**List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenantLicense]**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenantLicense.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_cache_tenant_response import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheTenantResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheTenantResponse from a JSON string
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_cache_tenant_response_instance = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheTenantResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheTenantResponse.to_json())

# convert the object into a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_cache_tenant_response_dict = ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_cache_tenant_response_instance.to_dict()
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheTenantResponse from a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_cache_tenant_response_from_dict = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheTenantResponse.from_dict(ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_cache_tenant_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


