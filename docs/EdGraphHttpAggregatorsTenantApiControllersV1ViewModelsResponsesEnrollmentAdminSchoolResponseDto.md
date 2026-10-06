# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminSchoolResponseDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**programs** | [**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminSchoolProgramResponseDto]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminSchoolProgramResponseDto.md) |  | [optional] 
**id** | **UUID** |  | [optional] 
**tenant_id** | **UUID** |  | [optional] 
**external_data_source_school_id** | **str** |  | [optional] 
**school_state_short_code** | **str** |  | [optional] 
**school_name** | **str** |  | [optional] 
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
**address_state_abbreviation** | **str** |  | [optional] 
**address_state** | **str** |  | [optional] 
**is_enabled** | **bool** |  | [optional] 
**program_count** | **int** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **datetime** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **datetime** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_school_response_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminSchoolResponseDto

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminSchoolResponseDto from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_school_response_dto_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminSchoolResponseDto.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminSchoolResponseDto.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_school_response_dto_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_school_response_dto_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminSchoolResponseDto from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_school_response_dto_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminSchoolResponseDto.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_school_response_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


