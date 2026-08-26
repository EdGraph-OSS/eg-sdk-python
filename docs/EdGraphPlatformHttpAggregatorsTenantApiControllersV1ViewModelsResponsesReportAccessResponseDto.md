# EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesReportAccessResponseDto

A report's audience targeting, returned with EdGraph.Platform.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Responses.ReportAccessResponseDto.TargetAudience as a stable  string (\"AnyoneInTenant\" | \"UsersWithRoleInTenant\" | \"SpecificUsersInTenant\") so the client  does not depend on proto enum serialization.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**report_id** | **str** |  | [optional] 
**target_audience** | **str** |  | [optional] 
**staff_classifications** | **List[str]** |  | [optional] 
**users** | **List[str]** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_report_access_response_dto import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesReportAccessResponseDto

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesReportAccessResponseDto from a JSON string
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_report_access_response_dto_instance = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesReportAccessResponseDto.from_json(json)
# print the JSON string representation of the object
print(EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesReportAccessResponseDto.to_json())

# convert the object into a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_report_access_response_dto_dict = ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_report_access_response_dto_instance.to_dict()
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesReportAccessResponseDto from a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_report_access_response_dto_from_dict = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesReportAccessResponseDto.from_dict(ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_report_access_response_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


