# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateSchoolProgramRequestDto

Covers two cases, distinguished by EdGraph.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Requests.EnrollmentAdmin.CreateSchoolProgramRequestDto.ProgramCatalogEntryId: adding an existing  district catalog entry to a school (a \"school association\" - EdGraph.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Requests.EnrollmentAdmin.CreateSchoolProgramRequestDto.Code/  EdGraph.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Requests.EnrollmentAdmin.CreateSchoolProgramRequestDto.Name/EdGraph.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Requests.EnrollmentAdmin.CreateSchoolProgramRequestDto.ProgramType/EdGraph.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Requests.EnrollmentAdmin.CreateSchoolProgramRequestDto.EligibilityCriteria/  EdGraph.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Requests.EnrollmentAdmin.CreateSchoolProgramRequestDto.RequiredDocuments are inherited and must be left unset), or creating a brand new  school-specific program (those same fields are required).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **UUID** |  | [optional] 
**school_code** | **str** |  | [optional] 
**school_name** | **str** |  | [optional] 
**program_catalog_entry_id** | **UUID** |  | [optional] 
**code** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**program_type** | **str** |  | [optional] 
**eligibility_criteria** | **str** |  | [optional] 
**required_documents** | **List[str]** |  | [optional] 
**grades** | **List[str]** |  | [optional] 
**capacity_by_grade** | [**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminGradeCapacityRequestDto]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminGradeCapacityRequestDto.md) |  | [optional] 
**zone** | **str** |  | [optional] 
**latitude** | **float** |  | [optional] 
**longitude** | **float** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_school_program_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateSchoolProgramRequestDto

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateSchoolProgramRequestDto from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_school_program_request_dto_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateSchoolProgramRequestDto.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateSchoolProgramRequestDto.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_school_program_request_dto_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_school_program_request_dto_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateSchoolProgramRequestDto from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_school_program_request_dto_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminCreateSchoolProgramRequestDto.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_create_school_program_request_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


