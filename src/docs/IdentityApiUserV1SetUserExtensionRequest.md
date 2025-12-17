# IdentityApiUserV1SetUserExtensionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**code** | **str** |  | [optional] 
**data** | **str** |  | [optional] 
**data_type** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_set_user_extension_request import IdentityApiUserV1SetUserExtensionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1SetUserExtensionRequest from a JSON string
identity_api_user_v1_set_user_extension_request_instance = IdentityApiUserV1SetUserExtensionRequest.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1SetUserExtensionRequest.to_json())

# convert the object into a dict
identity_api_user_v1_set_user_extension_request_dict = identity_api_user_v1_set_user_extension_request_instance.to_dict()
# create an instance of IdentityApiUserV1SetUserExtensionRequest from a dict
identity_api_user_v1_set_user_extension_request_from_dict = IdentityApiUserV1SetUserExtensionRequest.from_dict(identity_api_user_v1_set_user_extension_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


