# IdentityApiApiClientV1UpdateApiClientRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**client_name** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**api_claims** | [**List[IdentityApiApiClientV1ApiClaim]**](IdentityApiApiClientV1ApiClaim.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_api_client_v1_update_api_client_request import IdentityApiApiClientV1UpdateApiClientRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiApiClientV1UpdateApiClientRequest from a JSON string
identity_api_api_client_v1_update_api_client_request_instance = IdentityApiApiClientV1UpdateApiClientRequest.from_json(json)
# print the JSON string representation of the object
print(IdentityApiApiClientV1UpdateApiClientRequest.to_json())

# convert the object into a dict
identity_api_api_client_v1_update_api_client_request_dict = identity_api_api_client_v1_update_api_client_request_instance.to_dict()
# create an instance of IdentityApiApiClientV1UpdateApiClientRequest from a dict
identity_api_api_client_v1_update_api_client_request_from_dict = IdentityApiApiClientV1UpdateApiClientRequest.from_dict(identity_api_api_client_v1_update_api_client_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


