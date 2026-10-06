# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminWindowDependencyDto

\"Available only while window EdGraph.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Responses.EnrollmentAdmin.WindowDependencyDto.WindowId of round EdGraph.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Responses.EnrollmentAdmin.WindowDependencyDto.RoundId is EdGraph.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Responses.EnrollmentAdmin.WindowDependencyDto.WhenState\" (Open or Closed).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**round_id** | **UUID** |  | [optional] 
**window_id** | **UUID** |  | [optional] 
**when_state** | **str** |  | [optional] 
**unavailable_reason** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_window_dependency_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminWindowDependencyDto

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminWindowDependencyDto from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_window_dependency_dto_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminWindowDependencyDto.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminWindowDependencyDto.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_window_dependency_dto_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_window_dependency_dto_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminWindowDependencyDto from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_window_dependency_dto_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminWindowDependencyDto.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_window_dependency_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


