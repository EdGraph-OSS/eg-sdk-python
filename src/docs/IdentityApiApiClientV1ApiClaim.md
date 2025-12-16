# IdentityApiApiClientV1ApiClaim


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**application_id** | **str** |  | [optional] 
**subscription_id** | **str** |  | [optional] 
**value** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_api_client_v1_api_claim import IdentityApiApiClientV1ApiClaim

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiApiClientV1ApiClaim from a JSON string
identity_api_api_client_v1_api_claim_instance = IdentityApiApiClientV1ApiClaim.from_json(json)
# print the JSON string representation of the object
print(IdentityApiApiClientV1ApiClaim.to_json())

# convert the object into a dict
identity_api_api_client_v1_api_claim_dict = identity_api_api_client_v1_api_claim_instance.to_dict()
# create an instance of IdentityApiApiClientV1ApiClaim from a dict
identity_api_api_client_v1_api_claim_from_dict = IdentityApiApiClientV1ApiClaim.from_dict(identity_api_api_client_v1_api_claim_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


