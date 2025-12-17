# IdentityApiUserV1UserDeactivatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**user_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_user_deactivated_response import IdentityApiUserV1UserDeactivatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1UserDeactivatedResponse from a JSON string
identity_api_user_v1_user_deactivated_response_instance = IdentityApiUserV1UserDeactivatedResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1UserDeactivatedResponse.to_json())

# convert the object into a dict
identity_api_user_v1_user_deactivated_response_dict = identity_api_user_v1_user_deactivated_response_instance.to_dict()
# create an instance of IdentityApiUserV1UserDeactivatedResponse from a dict
identity_api_user_v1_user_deactivated_response_from_dict = IdentityApiUserV1UserDeactivatedResponse.from_dict(identity_api_user_v1_user_deactivated_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


