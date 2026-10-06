# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminEnrollmentWindowDto

A window the round owns. Instants are UTC; EdGraph.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Responses.EnrollmentAdmin.EnrollmentWindowDto.TimeZone is the IANA zone they are  shown in. EdGraph.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Responses.EnrollmentAdmin.EnrollmentWindowDto.OpensAt is absent when EdGraph.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Responses.EnrollmentAdmin.EnrollmentWindowDto.DependsOn sets the open moment.  EdGraph.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Responses.EnrollmentAdmin.EnrollmentWindowDto.UnavailableReason is present only while the dependency keeps the window closed.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | [optional] 
**kind** | **str** |  | [optional] 
**opens_at** | **datetime** |  | [optional] 
**closes_at** | **datetime** |  | [optional] 
**time_zone** | **str** |  | [optional] 
**depends_on** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminWindowDependencyDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminWindowDependencyDto.md) |  | [optional] 
**state** | **str** |  | [optional] 
**unavailable_reason** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_enrollment_window_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminEnrollmentWindowDto

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminEnrollmentWindowDto from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_enrollment_window_dto_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminEnrollmentWindowDto.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminEnrollmentWindowDto.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_enrollment_window_dto_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_enrollment_window_dto_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminEnrollmentWindowDto from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_enrollment_window_dto_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminEnrollmentWindowDto.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_enrollment_window_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


