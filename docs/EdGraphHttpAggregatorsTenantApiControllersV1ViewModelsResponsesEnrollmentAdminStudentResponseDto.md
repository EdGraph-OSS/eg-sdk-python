# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminStudentResponseDto

One Enrollment Student, from the list and the get-by-id route alike. `registrationId` is set only on  a list row that stands for a registration not yet linked to a student (a new student): that row's  `id` is the registration's id, which the get-by-id route cannot resolve, so a client must not open a  student profile from it. Absent on every real student.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | [optional] 
**tenant_id** | **UUID** |  | [optional] 
**student_local_code** | **str** |  | [optional] 
**student_state_code** | **str** |  | [optional] 
**external_data_source_student_id** | **str** |  | [optional] 
**allowed_pathway_ids** | [**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminAllowedPathwayIdDto]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminAllowedPathwayIdDto.md) |  | [optional] 
**first_name** | **str** |  | [optional] 
**middle_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**birthdate** | **str** |  | [optional] 
**last4_ssn** | **str** |  | [optional] 
**next_address** | **str** |  | [optional] 
**next_grade_level** | **str** |  | [optional] 
**next_school_state_short_code** | **str** |  | [optional] 
**next_school_state_code** | **str** |  | [optional] 
**next_school_name** | **str** |  | [optional] 
**next_school_address** | **str** |  | [optional] 
**eligibility_code** | **str** |  | [optional] 
**eligibility_description** | **str** |  | [optional] 
**contacts** | [**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminStudentContactResponseDto]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminStudentContactResponseDto.md) |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **datetime** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **datetime** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **datetime** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**registration_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_student_response_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminStudentResponseDto

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminStudentResponseDto from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_student_response_dto_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminStudentResponseDto.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminStudentResponseDto.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_student_response_dto_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_student_response_dto_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminStudentResponseDto from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_student_response_dto_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesEnrollmentAdminStudentResponseDto.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_enrollment_admin_student_response_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


