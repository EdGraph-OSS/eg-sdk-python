# IdentityApiUserV1Preference


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**code** | **str** |  | [optional] 
**value** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_preference import IdentityApiUserV1Preference

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1Preference from a JSON string
identity_api_user_v1_preference_instance = IdentityApiUserV1Preference.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1Preference.to_json())

# convert the object into a dict
identity_api_user_v1_preference_dict = identity_api_user_v1_preference_instance.to_dict()
# create an instance of IdentityApiUserV1Preference from a dict
identity_api_user_v1_preference_from_dict = IdentityApiUserV1Preference.from_dict(identity_api_user_v1_preference_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


