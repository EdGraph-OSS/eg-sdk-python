# IdentityApiUserV1UserLogin


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**login_provider** | **str** |  | [optional] 
**provider_display_name** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_user_login import IdentityApiUserV1UserLogin

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1UserLogin from a JSON string
identity_api_user_v1_user_login_instance = IdentityApiUserV1UserLogin.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1UserLogin.to_json())

# convert the object into a dict
identity_api_user_v1_user_login_dict = identity_api_user_v1_user_login_instance.to_dict()
# create an instance of IdentityApiUserV1UserLogin from a dict
identity_api_user_v1_user_login_from_dict = IdentityApiUserV1UserLogin.from_dict(identity_api_user_v1_user_login_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


