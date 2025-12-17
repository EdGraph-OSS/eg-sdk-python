# EdfiAdminApiEdfiAdminV1StudentEnrollmentByGenderReportResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**local_education_agency_id** | **int** |  | [optional] 
**local_education_agency_name** | **str** |  | [optional] 
**total_student_count** | **int** |  | [optional] 
**gender_representation** | [**List[EdfiAdminApiEdfiAdminV1GenderRepresentation]**](EdfiAdminApiEdfiAdminV1GenderRepresentation.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_student_enrollment_by_gender_report_response import EdfiAdminApiEdfiAdminV1StudentEnrollmentByGenderReportResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1StudentEnrollmentByGenderReportResponse from a JSON string
edfi_admin_api_edfi_admin_v1_student_enrollment_by_gender_report_response_instance = EdfiAdminApiEdfiAdminV1StudentEnrollmentByGenderReportResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1StudentEnrollmentByGenderReportResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_student_enrollment_by_gender_report_response_dict = edfi_admin_api_edfi_admin_v1_student_enrollment_by_gender_report_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1StudentEnrollmentByGenderReportResponse from a dict
edfi_admin_api_edfi_admin_v1_student_enrollment_by_gender_report_response_from_dict = EdfiAdminApiEdfiAdminV1StudentEnrollmentByGenderReportResponse.from_dict(edfi_admin_api_edfi_admin_v1_student_enrollment_by_gender_report_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


