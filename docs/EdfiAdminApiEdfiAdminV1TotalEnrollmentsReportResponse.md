# EdfiAdminApiEdfiAdminV1TotalEnrollmentsReportResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enrollment_count** | **int** |  | [optional] 
**education_organization_id** | **int** |  | [optional] 
**id** | **str** |  | [optional] 
**name_of_institution** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_total_enrollments_report_response import EdfiAdminApiEdfiAdminV1TotalEnrollmentsReportResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1TotalEnrollmentsReportResponse from a JSON string
edfi_admin_api_edfi_admin_v1_total_enrollments_report_response_instance = EdfiAdminApiEdfiAdminV1TotalEnrollmentsReportResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1TotalEnrollmentsReportResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_total_enrollments_report_response_dict = edfi_admin_api_edfi_admin_v1_total_enrollments_report_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1TotalEnrollmentsReportResponse from a dict
edfi_admin_api_edfi_admin_v1_total_enrollments_report_response_from_dict = EdfiAdminApiEdfiAdminV1TotalEnrollmentsReportResponse.from_dict(edfi_admin_api_edfi_admin_v1_total_enrollments_report_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


