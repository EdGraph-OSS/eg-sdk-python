# EdfiAdminApiEdfiAdminV1EducationOrganizationAddress


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address_type_descriptor** | **str** |  | [optional] 
**state_abbreviation_descriptor** | **str** |  | [optional] 
**city** | **str** |  | [optional] 
**postal_code** | **str** |  | [optional] 
**street_number_name** | **str** |  | [optional] 
**locale_descriptor** | **str** |  | [optional] 
**building_site_number** | **str** |  | [optional] 
**name_of_county** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_education_organization_address import EdfiAdminApiEdfiAdminV1EducationOrganizationAddress

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1EducationOrganizationAddress from a JSON string
edfi_admin_api_edfi_admin_v1_education_organization_address_instance = EdfiAdminApiEdfiAdminV1EducationOrganizationAddress.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1EducationOrganizationAddress.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_education_organization_address_dict = edfi_admin_api_edfi_admin_v1_education_organization_address_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1EducationOrganizationAddress from a dict
edfi_admin_api_edfi_admin_v1_education_organization_address_from_dict = EdfiAdminApiEdfiAdminV1EducationOrganizationAddress.from_dict(edfi_admin_api_edfi_admin_v1_education_organization_address_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


