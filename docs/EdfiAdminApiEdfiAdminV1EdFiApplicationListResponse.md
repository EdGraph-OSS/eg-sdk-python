# EdfiAdminApiEdfiAdminV1EdFiApplicationListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**application_id** | **int** |  | [optional] 
**application_name** | **str** |  | [optional] 
**claim_set_name** | **str** |  | [optional] 
**vendor_id** | **int** |  | [optional] 
**vendor_name** | **str** |  | [optional] 
**ed_orgs_count** | **int** |  | [optional] 
**operational_context_uri** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ed_fi_application_list_response import EdfiAdminApiEdfiAdminV1EdFiApplicationListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1EdFiApplicationListResponse from a JSON string
edfi_admin_api_edfi_admin_v1_ed_fi_application_list_response_instance = EdfiAdminApiEdfiAdminV1EdFiApplicationListResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1EdFiApplicationListResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_ed_fi_application_list_response_dict = edfi_admin_api_edfi_admin_v1_ed_fi_application_list_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1EdFiApplicationListResponse from a dict
edfi_admin_api_edfi_admin_v1_ed_fi_application_list_response_from_dict = EdfiAdminApiEdfiAdminV1EdFiApplicationListResponse.from_dict(edfi_admin_api_edfi_admin_v1_ed_fi_application_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


