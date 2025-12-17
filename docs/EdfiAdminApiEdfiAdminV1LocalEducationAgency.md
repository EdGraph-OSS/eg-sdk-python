# EdfiAdminApiEdfiAdminV1LocalEducationAgency


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**education_organization_id** | **int** |  | [optional] 
**local_education_agency_id** | **int** |  | [optional] 
**name_of_institution** | **str** |  | [optional] 
**shortname_of_institution** | **str** |  | [optional] 
**web_site** | **str** |  | [optional] 
**operational_status_descriptor_id** | **int** |  | [optional] 
**discriminator** | **str** |  | [optional] 
**create_date** | **str** |  | [optional] 
**last_modified_date** | **str** |  | [optional] 
**addresses** | [**List[EdfiAdminApiEdfiAdminV1EducationOrganizationAddress]**](EdfiAdminApiEdfiAdminV1EducationOrganizationAddress.md) |  | [optional] [readonly] 
**categories** | [**List[EdfiAdminApiEdfiAdminV1EducationOrganizationCategoryDescriptor]**](EdfiAdminApiEdfiAdminV1EducationOrganizationCategoryDescriptor.md) |  | [optional] [readonly] 
**local_education_agency_category_descriptor_code_value** | **str** |  | [optional] 
**id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_local_education_agency import EdfiAdminApiEdfiAdminV1LocalEducationAgency

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1LocalEducationAgency from a JSON string
edfi_admin_api_edfi_admin_v1_local_education_agency_instance = EdfiAdminApiEdfiAdminV1LocalEducationAgency.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1LocalEducationAgency.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_local_education_agency_dict = edfi_admin_api_edfi_admin_v1_local_education_agency_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1LocalEducationAgency from a dict
edfi_admin_api_edfi_admin_v1_local_education_agency_from_dict = EdfiAdminApiEdfiAdminV1LocalEducationAgency.from_dict(edfi_admin_api_edfi_admin_v1_local_education_agency_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


