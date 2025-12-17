# EdfiAdminApiEdfiAdminV1EdFiApplicationApiClientProfileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**api_client_id** | **int** |  | [optional] 
**key** | **str** |  | [optional] 
**secret** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**is_approved** | **bool** |  | [optional] 
**use_sandbox** | **bool** |  | [optional] 
**sandbox_type** | **int** |  | [optional] 
**application_id** | **int** |  | [optional] 
**secret_is_hashed** | **bool** |  | [optional] 
**key_status** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ed_fi_application_api_client_profile_response import EdfiAdminApiEdfiAdminV1EdFiApplicationApiClientProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1EdFiApplicationApiClientProfileResponse from a JSON string
edfi_admin_api_edfi_admin_v1_ed_fi_application_api_client_profile_response_instance = EdfiAdminApiEdfiAdminV1EdFiApplicationApiClientProfileResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1EdFiApplicationApiClientProfileResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_ed_fi_application_api_client_profile_response_dict = edfi_admin_api_edfi_admin_v1_ed_fi_application_api_client_profile_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1EdFiApplicationApiClientProfileResponse from a dict
edfi_admin_api_edfi_admin_v1_ed_fi_application_api_client_profile_response_from_dict = EdfiAdminApiEdfiAdminV1EdFiApplicationApiClientProfileResponse.from_dict(edfi_admin_api_edfi_admin_v1_ed_fi_application_api_client_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


