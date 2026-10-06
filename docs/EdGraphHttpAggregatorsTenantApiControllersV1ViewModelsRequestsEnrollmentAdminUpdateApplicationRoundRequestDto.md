# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateApplicationRoundRequestDto

Replaces label, grades and program types. Code and school year are the round's identity and  cannot change - duplicate the round into another school year instead.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | [optional] 
**tenant_id** | **UUID** |  | [optional] 
**label** | **str** |  | [optional] 
**grades** | **List[str]** |  | [optional] 
**program_type_ids** | **List[UUID]** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_application_round_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateApplicationRoundRequestDto

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateApplicationRoundRequestDto from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_application_round_request_dto_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateApplicationRoundRequestDto.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateApplicationRoundRequestDto.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_application_round_request_dto_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_application_round_request_dto_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateApplicationRoundRequestDto from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_application_round_request_dto_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateApplicationRoundRequestDto.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_application_round_request_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


