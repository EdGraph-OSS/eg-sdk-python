# EdfiAdminApiEdfiAdminV1EducationOrganization


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**education_organization_id** | **int** |  | [optional] 
**name_of_institution** | **str** |  | [optional] 
**shortname_of_institution** | **str** |  | [optional] 
**web_site** | **str** |  | [optional] 
**operational_status_descriptor_id** | **int** |  | [optional] 
**discriminator** | **str** |  | [optional] 
**create_date** | **str** |  | [optional] 
**last_modified_date** | **str** |  | [optional] 
**id** | **str** |  | [optional] 
**change_version** | **int** |  | [optional] 
**created_by_ownership_token_id** | **int** |  | [optional] 
**local_education_agency_id** | **int** |  | [optional] 
**school_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_education_organization import EdfiAdminApiEdfiAdminV1EducationOrganization

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1EducationOrganization from a JSON string
edfi_admin_api_edfi_admin_v1_education_organization_instance = EdfiAdminApiEdfiAdminV1EducationOrganization.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1EducationOrganization.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_education_organization_dict = edfi_admin_api_edfi_admin_v1_education_organization_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1EducationOrganization from a dict
edfi_admin_api_edfi_admin_v1_education_organization_from_dict = EdfiAdminApiEdfiAdminV1EducationOrganization.from_dict(edfi_admin_api_edfi_admin_v1_education_organization_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


