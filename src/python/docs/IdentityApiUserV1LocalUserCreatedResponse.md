# IdentityApiUserV1LocalUserCreatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**user_id** | **str** |  | [optional] 
**password** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_local_user_created_response import IdentityApiUserV1LocalUserCreatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1LocalUserCreatedResponse from a JSON string
identity_api_user_v1_local_user_created_response_instance = IdentityApiUserV1LocalUserCreatedResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1LocalUserCreatedResponse.to_json())

# convert the object into a dict
identity_api_user_v1_local_user_created_response_dict = identity_api_user_v1_local_user_created_response_instance.to_dict()
# create an instance of IdentityApiUserV1LocalUserCreatedResponse from a dict
identity_api_user_v1_local_user_created_response_from_dict = IdentityApiUserV1LocalUserCreatedResponse.from_dict(identity_api_user_v1_local_user_created_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


