# EdfiAdminApiEdfiAdminV1EducationServiceCenter


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**education_service_center_id** | **int** |  | [optional] 
**name_of_institution** | **str** |  | [optional] 
**education_organization_category_descriptors** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_education_service_center import EdfiAdminApiEdfiAdminV1EducationServiceCenter

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1EducationServiceCenter from a JSON string
edfi_admin_api_edfi_admin_v1_education_service_center_instance = EdfiAdminApiEdfiAdminV1EducationServiceCenter.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1EducationServiceCenter.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_education_service_center_dict = edfi_admin_api_edfi_admin_v1_education_service_center_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1EducationServiceCenter from a dict
edfi_admin_api_edfi_admin_v1_education_service_center_from_dict = EdfiAdminApiEdfiAdminV1EducationServiceCenter.from_dict(edfi_admin_api_edfi_admin_v1_education_service_center_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


