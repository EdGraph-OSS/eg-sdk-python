# IdentityApiApiClientV1Claim


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**value** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_api_client_v1_claim import IdentityApiApiClientV1Claim

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiApiClientV1Claim from a JSON string
identity_api_api_client_v1_claim_instance = IdentityApiApiClientV1Claim.from_json(json)
# print the JSON string representation of the object
print(IdentityApiApiClientV1Claim.to_json())

# convert the object into a dict
identity_api_api_client_v1_claim_dict = identity_api_api_client_v1_claim_instance.to_dict()
# create an instance of IdentityApiApiClientV1Claim from a dict
identity_api_api_client_v1_claim_from_dict = IdentityApiApiClientV1Claim.from_dict(identity_api_api_client_v1_claim_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


