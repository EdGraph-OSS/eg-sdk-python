# EdfiAdminApiEdfiAdminV1SchoolsByTypeReportResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**school_count_representations** | [**List[EdfiAdminApiEdfiAdminV1SchoolCountRepresentation]**](EdfiAdminApiEdfiAdminV1SchoolCountRepresentation.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_schools_by_type_report_response import EdfiAdminApiEdfiAdminV1SchoolsByTypeReportResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1SchoolsByTypeReportResponse from a JSON string
edfi_admin_api_edfi_admin_v1_schools_by_type_report_response_instance = EdfiAdminApiEdfiAdminV1SchoolsByTypeReportResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1SchoolsByTypeReportResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_schools_by_type_report_response_dict = edfi_admin_api_edfi_admin_v1_schools_by_type_report_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1SchoolsByTypeReportResponse from a dict
edfi_admin_api_edfi_admin_v1_schools_by_type_report_response_from_dict = EdfiAdminApiEdfiAdminV1SchoolsByTypeReportResponse.from_dict(edfi_admin_api_edfi_admin_v1_schools_by_type_report_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


