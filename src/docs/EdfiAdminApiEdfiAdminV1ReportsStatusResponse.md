# EdfiAdminApiEdfiAdminV1ReportsStatusResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**district_schools_by_type_report** | **bool** |  | [optional] 
**district_total_enrollments_report** | **bool** |  | [optional] 
**local_education_agencies_report** | **bool** |  | [optional] 
**student_demographics_report** | **bool** |  | [optional] 
**student_economic_situation_report** | **bool** |  | [optional] 
**students_by_program_report** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_reports_status_response import EdfiAdminApiEdfiAdminV1ReportsStatusResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1ReportsStatusResponse from a JSON string
edfi_admin_api_edfi_admin_v1_reports_status_response_instance = EdfiAdminApiEdfiAdminV1ReportsStatusResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1ReportsStatusResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_reports_status_response_dict = edfi_admin_api_edfi_admin_v1_reports_status_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1ReportsStatusResponse from a dict
edfi_admin_api_edfi_admin_v1_reports_status_response_from_dict = EdfiAdminApiEdfiAdminV1ReportsStatusResponse.from_dict(edfi_admin_api_edfi_admin_v1_reports_status_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


