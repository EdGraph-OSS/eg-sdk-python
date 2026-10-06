# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminEnrollmentWindowRequestDto

A window as written. EdGraph.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Requests.EnrollmentAdmin.EnrollmentWindowRequestDto.OpensAt and EdGraph.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Requests.EnrollmentAdmin.EnrollmentWindowRequestDto.ClosesAt are ISO-8601 instants with  their offset (\"2026-06-01T08:00:00-05:00\" or \"...Z\"); they are passed to the Enrollment Service  verbatim, which refuses one without an offset. EdGraph.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Requests.EnrollmentAdmin.EnrollmentWindowRequestDto.OpensAt may be omitted only when  EdGraph.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Requests.EnrollmentAdmin.EnrollmentWindowRequestDto.DependsOn is set.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**kind** | **str** |  | [optional] 
**opens_at** | **str** |  | [optional] 
**closes_at** | **str** |  | [optional] 
**time_zone** | **str** |  | [optional] 
**depends_on** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminWindowDependencyRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminWindowDependencyRequestDto.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminEnrollmentWindowRequestDto

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminEnrollmentWindowRequestDto from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminEnrollmentWindowRequestDto.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminEnrollmentWindowRequestDto.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminEnrollmentWindowRequestDto from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminEnrollmentWindowRequestDto.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_enrollment_window_request_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


