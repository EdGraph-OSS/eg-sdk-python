# IdentityApiUserV1DeactivateUserRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**user_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_deactivate_user_request import IdentityApiUserV1DeactivateUserRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1DeactivateUserRequest from a JSON string
identity_api_user_v1_deactivate_user_request_instance = IdentityApiUserV1DeactivateUserRequest.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1DeactivateUserRequest.to_json())

# convert the object into a dict
identity_api_user_v1_deactivate_user_request_dict = identity_api_user_v1_deactivate_user_request_instance.to_dict()
# create an instance of IdentityApiUserV1DeactivateUserRequest from a dict
identity_api_user_v1_deactivate_user_request_from_dict = IdentityApiUserV1DeactivateUserRequest.from_dict(identity_api_user_v1_deactivate_user_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


