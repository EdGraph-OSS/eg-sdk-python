# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpsertSchoolRequestDto

The body of a school creation or update.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **UUID** | Must match the tenant in the route. | [optional] 
**external_data_source_school_id** | **str** | When present, the upsert is keyed on this id rather than SchoolStateShortCode:  a live school with a matching external id is updated; a soft-deleted one is refused (recover it  first). When absent, a new school is always inserted, and a SchoolStateShortCode  collision on insert is rejected as AlreadyExists. | [optional] 
**school_state_short_code** | **str** | Required. Unique per tenant. | [optional] 
**school_name** | **str** | Required. | [optional] 
**district_state_short_code** | **str** |  | [optional] 
**school_state_long_code** | **str** |  | [optional] 
**school_local_code** | **str** |  | [optional] 
**district_local_code** | **str** |  | [optional] 
**district_state_code** | **str** |  | [optional] 
**district_name** | **str** |  | [optional] 
**grades_served** | **List[str]** |  | [optional] 
**address** | **str** |  | [optional] 
**lat** | **float** |  | [optional] 
**lon** | **float** |  | [optional] 
**phone** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_upsert_school_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpsertSchoolRequestDto

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpsertSchoolRequestDto from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_upsert_school_request_dto_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpsertSchoolRequestDto.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpsertSchoolRequestDto.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_upsert_school_request_dto_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_upsert_school_request_dto_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpsertSchoolRequestDto from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_upsert_school_request_dto_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpsertSchoolRequestDto.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_upsert_school_request_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


