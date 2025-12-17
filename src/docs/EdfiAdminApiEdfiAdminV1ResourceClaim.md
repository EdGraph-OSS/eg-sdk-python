# EdfiAdminApiEdfiAdminV1ResourceClaim


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**resource_claim_id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**create** | **bool** |  | [optional] 
**create_auth_strategy** | **str** |  | [optional] 
**read** | **bool** |  | [optional] 
**read_auth_strategy** | **str** |  | [optional] 
**update** | **bool** |  | [optional] 
**update_auth_strategy** | **str** |  | [optional] 
**delete** | **bool** |  | [optional] 
**delete_auth_strategy** | **str** |  | [optional] 
**children** | [**List[EdfiAdminApiEdfiAdminV1ResourceClaim]**](EdfiAdminApiEdfiAdminV1ResourceClaim.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_resource_claim import EdfiAdminApiEdfiAdminV1ResourceClaim

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1ResourceClaim from a JSON string
edfi_admin_api_edfi_admin_v1_resource_claim_instance = EdfiAdminApiEdfiAdminV1ResourceClaim.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1ResourceClaim.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_resource_claim_dict = edfi_admin_api_edfi_admin_v1_resource_claim_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1ResourceClaim from a dict
edfi_admin_api_edfi_admin_v1_resource_claim_from_dict = EdfiAdminApiEdfiAdminV1ResourceClaim.from_dict(edfi_admin_api_edfi_admin_v1_resource_claim_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


