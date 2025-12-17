# EdfiAdminApiEdfiAdminV1ClaimSetDetailsResourceClaim


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**resource_claim_id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**create** | **bool** |  | [optional] 
**create_auth_strategy** | **str** |  | [optional] 
**create_auth_strategy_override** | **str** |  | [optional] 
**read** | **bool** |  | [optional] 
**read_auth_strategy** | **str** |  | [optional] 
**read_auth_strategy_override** | **str** |  | [optional] 
**update** | **bool** |  | [optional] 
**update_auth_strategy** | **str** |  | [optional] 
**update_auth_strategy_override** | **str** |  | [optional] 
**delete** | **bool** |  | [optional] 
**delete_auth_strategy** | **str** |  | [optional] 
**delete_auth_strategy_override** | **str** |  | [optional] 
**children** | [**List[EdfiAdminApiEdfiAdminV1ClaimSetDetailsResourceClaim]**](EdfiAdminApiEdfiAdminV1ClaimSetDetailsResourceClaim.md) |  | [optional] [readonly] 
**read_changes** | **bool** |  | [optional] 
**read_changes_auth_strategy** | **str** |  | [optional] 
**read_changes_auth_strategy_override** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_claim_set_details_resource_claim import EdfiAdminApiEdfiAdminV1ClaimSetDetailsResourceClaim

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1ClaimSetDetailsResourceClaim from a JSON string
edfi_admin_api_edfi_admin_v1_claim_set_details_resource_claim_instance = EdfiAdminApiEdfiAdminV1ClaimSetDetailsResourceClaim.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1ClaimSetDetailsResourceClaim.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_claim_set_details_resource_claim_dict = edfi_admin_api_edfi_admin_v1_claim_set_details_resource_claim_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1ClaimSetDetailsResourceClaim from a dict
edfi_admin_api_edfi_admin_v1_claim_set_details_resource_claim_from_dict = EdfiAdminApiEdfiAdminV1ClaimSetDetailsResourceClaim.from_dict(edfi_admin_api_edfi_admin_v1_claim_set_details_resource_claim_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


