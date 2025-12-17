# EdfiAdminApiEdfiAdminV1StateEducationAgency


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**state_education_agency_id** | **int** |  | [optional] 
**name_of_institution** | **str** |  | [optional] 
**education_organization_category_descriptors** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_state_education_agency import EdfiAdminApiEdfiAdminV1StateEducationAgency

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1StateEducationAgency from a JSON string
edfi_admin_api_edfi_admin_v1_state_education_agency_instance = EdfiAdminApiEdfiAdminV1StateEducationAgency.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1StateEducationAgency.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_state_education_agency_dict = edfi_admin_api_edfi_admin_v1_state_education_agency_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1StateEducationAgency from a dict
edfi_admin_api_edfi_admin_v1_state_education_agency_from_dict = EdfiAdminApiEdfiAdminV1StateEducationAgency.from_dict(edfi_admin_api_edfi_admin_v1_state_education_agency_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


