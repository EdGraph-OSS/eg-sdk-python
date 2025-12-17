# EdfiAdminApiEdfiAdminV1UpdateEdFiApplicationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**application_id** | **int** |  | [optional] 
**application_name** | **str** |  | [optional] 
**claim_set_name** | **str** |  | [optional] 
**vendor_id** | **int** |  | [optional] 
**education_organizations** | [**List[EdfiAdminApiEdfiAdminV1EducationOrganization]**](EdfiAdminApiEdfiAdminV1EducationOrganization.md) |  | [optional] [readonly] 
**operational_context_uri** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_ed_fi_application_request import EdfiAdminApiEdfiAdminV1UpdateEdFiApplicationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1UpdateEdFiApplicationRequest from a JSON string
edfi_admin_api_edfi_admin_v1_update_ed_fi_application_request_instance = EdfiAdminApiEdfiAdminV1UpdateEdFiApplicationRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1UpdateEdFiApplicationRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_update_ed_fi_application_request_dict = edfi_admin_api_edfi_admin_v1_update_ed_fi_application_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1UpdateEdFiApplicationRequest from a dict
edfi_admin_api_edfi_admin_v1_update_ed_fi_application_request_from_dict = EdfiAdminApiEdfiAdminV1UpdateEdFiApplicationRequest.from_dict(edfi_admin_api_edfi_admin_v1_update_ed_fi_application_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


