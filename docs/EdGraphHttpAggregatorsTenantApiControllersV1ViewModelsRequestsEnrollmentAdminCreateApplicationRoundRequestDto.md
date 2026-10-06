# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateApplicationRoundRequestDto

Creates a round. Windows are added afterwards, one at a time.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **UUID** |  | [optional] 
**code** | **str** |  | [optional] 
**school_year** | **str** |  | [optional] 
**label** | **str** |  | [optional] 
**grades** | **List[str]** |  | [optional] 
**program_type_ids** | **List[UUID]** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_application_round_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateApplicationRoundRequestDto

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateApplicationRoundRequestDto from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_application_round_request_dto_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateApplicationRoundRequestDto.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateApplicationRoundRequestDto.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_application_round_request_dto_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_application_round_request_dto_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateApplicationRoundRequestDto from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_application_round_request_dto_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateApplicationRoundRequestDto.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_application_round_request_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


