# EdfiAdminApiEdfiAdminV1AddSchoolYearRangeRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**entries** | [**List[EdfiAdminApiEdfiAdminV1AddSchoolYearRangeRequestEntry]**](EdfiAdminApiEdfiAdminV1AddSchoolYearRangeRequestEntry.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_add_school_year_range_request import EdfiAdminApiEdfiAdminV1AddSchoolYearRangeRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1AddSchoolYearRangeRequest from a JSON string
edfi_admin_api_edfi_admin_v1_add_school_year_range_request_instance = EdfiAdminApiEdfiAdminV1AddSchoolYearRangeRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1AddSchoolYearRangeRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_add_school_year_range_request_dict = edfi_admin_api_edfi_admin_v1_add_school_year_range_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1AddSchoolYearRangeRequest from a dict
edfi_admin_api_edfi_admin_v1_add_school_year_range_request_from_dict = EdfiAdminApiEdfiAdminV1AddSchoolYearRangeRequest.from_dict(edfi_admin_api_edfi_admin_v1_add_school_year_range_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


