# EdfiAdminApiEdfiAdminV1EdFiApplicationProfileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**application_id** | **int** |  | [optional] 
**application_name** | **str** |  | [optional] 
**claim_set_name** | **str** |  | [optional] 
**vendor_id** | **int** |  | [optional] 
**vendor** | [**EdfiAdminApiEdfiAdminV1Vendor**](EdfiAdminApiEdfiAdminV1Vendor.md) |  | [optional] 
**education_organizations** | [**List[EdfiAdminApiEdfiAdminV1EducationOrganization]**](EdfiAdminApiEdfiAdminV1EducationOrganization.md) | TODO Is adding Vendor object which also has application object correct ? | [optional] [readonly] 
**operational_context_uri** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ed_fi_application_profile_response import EdfiAdminApiEdfiAdminV1EdFiApplicationProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1EdFiApplicationProfileResponse from a JSON string
edfi_admin_api_edfi_admin_v1_ed_fi_application_profile_response_instance = EdfiAdminApiEdfiAdminV1EdFiApplicationProfileResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1EdFiApplicationProfileResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_ed_fi_application_profile_response_dict = edfi_admin_api_edfi_admin_v1_ed_fi_application_profile_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1EdFiApplicationProfileResponse from a dict
edfi_admin_api_edfi_admin_v1_ed_fi_application_profile_response_from_dict = EdfiAdminApiEdfiAdminV1EdFiApplicationProfileResponse.from_dict(edfi_admin_api_edfi_admin_v1_ed_fi_application_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


