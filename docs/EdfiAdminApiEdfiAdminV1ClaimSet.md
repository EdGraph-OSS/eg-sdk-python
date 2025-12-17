# EdfiAdminApiEdfiAdminV1ClaimSet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**claim_set_id** | **int** |  | [optional] 
**claim_set_name** | **str** |  | [optional] 
**is_system_reserved** | **bool** |  | [optional] 
**applications_count** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_claim_set import EdfiAdminApiEdfiAdminV1ClaimSet

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1ClaimSet from a JSON string
edfi_admin_api_edfi_admin_v1_claim_set_instance = EdfiAdminApiEdfiAdminV1ClaimSet.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1ClaimSet.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_claim_set_dict = edfi_admin_api_edfi_admin_v1_claim_set_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1ClaimSet from a dict
edfi_admin_api_edfi_admin_v1_claim_set_from_dict = EdfiAdminApiEdfiAdminV1ClaimSet.from_dict(edfi_admin_api_edfi_admin_v1_claim_set_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


