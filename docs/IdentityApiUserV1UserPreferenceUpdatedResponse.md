# IdentityApiUserV1UserPreferenceUpdatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**code** | **str** |  | [optional] 
**value** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_user_preference_updated_response import IdentityApiUserV1UserPreferenceUpdatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1UserPreferenceUpdatedResponse from a JSON string
identity_api_user_v1_user_preference_updated_response_instance = IdentityApiUserV1UserPreferenceUpdatedResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1UserPreferenceUpdatedResponse.to_json())

# convert the object into a dict
identity_api_user_v1_user_preference_updated_response_dict = identity_api_user_v1_user_preference_updated_response_instance.to_dict()
# create an instance of IdentityApiUserV1UserPreferenceUpdatedResponse from a dict
identity_api_user_v1_user_preference_updated_response_from_dict = IdentityApiUserV1UserPreferenceUpdatedResponse.from_dict(identity_api_user_v1_user_preference_updated_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


