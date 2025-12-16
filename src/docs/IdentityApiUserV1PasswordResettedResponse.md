# IdentityApiUserV1PasswordResettedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**user_id** | **str** |  | [optional] 
**password** | **str** |  | [optional] 
**auto_generated_password** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_password_resetted_response import IdentityApiUserV1PasswordResettedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1PasswordResettedResponse from a JSON string
identity_api_user_v1_password_resetted_response_instance = IdentityApiUserV1PasswordResettedResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1PasswordResettedResponse.to_json())

# convert the object into a dict
identity_api_user_v1_password_resetted_response_dict = identity_api_user_v1_password_resetted_response_instance.to_dict()
# create an instance of IdentityApiUserV1PasswordResettedResponse from a dict
identity_api_user_v1_password_resetted_response_from_dict = IdentityApiUserV1PasswordResettedResponse.from_dict(identity_api_user_v1_password_resetted_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


