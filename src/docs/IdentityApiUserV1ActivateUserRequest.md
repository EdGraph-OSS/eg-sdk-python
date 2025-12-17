# IdentityApiUserV1ActivateUserRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**user_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_activate_user_request import IdentityApiUserV1ActivateUserRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1ActivateUserRequest from a JSON string
identity_api_user_v1_activate_user_request_instance = IdentityApiUserV1ActivateUserRequest.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1ActivateUserRequest.to_json())

# convert the object into a dict
identity_api_user_v1_activate_user_request_dict = identity_api_user_v1_activate_user_request_instance.to_dict()
# create an instance of IdentityApiUserV1ActivateUserRequest from a dict
identity_api_user_v1_activate_user_request_from_dict = IdentityApiUserV1ActivateUserRequest.from_dict(identity_api_user_v1_activate_user_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


