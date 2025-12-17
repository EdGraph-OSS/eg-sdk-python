# EdfiAdminApiEdfiAdminV1SaveClaimSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**claim_set_id** | **int** |  | [optional] 
**claim_set_name** | **str** |  | [optional] 
**application_id** | **int** |  | [optional] 
**resource_claims** | [**List[EdfiAdminApiEdfiAdminV1ClaimSetDetailsResourceClaim]**](EdfiAdminApiEdfiAdminV1ClaimSetDetailsResourceClaim.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_save_claim_set_request import EdfiAdminApiEdfiAdminV1SaveClaimSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1SaveClaimSetRequest from a JSON string
edfi_admin_api_edfi_admin_v1_save_claim_set_request_instance = EdfiAdminApiEdfiAdminV1SaveClaimSetRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1SaveClaimSetRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_save_claim_set_request_dict = edfi_admin_api_edfi_admin_v1_save_claim_set_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1SaveClaimSetRequest from a dict
edfi_admin_api_edfi_admin_v1_save_claim_set_request_from_dict = EdfiAdminApiEdfiAdminV1SaveClaimSetRequest.from_dict(edfi_admin_api_edfi_admin_v1_save_claim_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


