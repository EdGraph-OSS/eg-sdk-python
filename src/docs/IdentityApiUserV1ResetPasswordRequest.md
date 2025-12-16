# IdentityApiUserV1ResetPasswordRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**user_id** | **str** |  | [optional] 
**password** | **str** |  | [optional] 
**auto_generated_password** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_reset_password_request import IdentityApiUserV1ResetPasswordRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1ResetPasswordRequest from a JSON string
identity_api_user_v1_reset_password_request_instance = IdentityApiUserV1ResetPasswordRequest.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1ResetPasswordRequest.to_json())

# convert the object into a dict
identity_api_user_v1_reset_password_request_dict = identity_api_user_v1_reset_password_request_instance.to_dict()
# create an instance of IdentityApiUserV1ResetPasswordRequest from a dict
identity_api_user_v1_reset_password_request_from_dict = IdentityApiUserV1ResetPasswordRequest.from_dict(identity_api_user_v1_reset_password_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


