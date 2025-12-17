# IdentityApiUserV2UserMeProfile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**user_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**tenant_count** | **int** |  | [optional] 
**extensions** | [**List[IdentityApiUserV2UserExtension]**](IdentityApiUserV2UserExtension.md) |  | [optional] [readonly] 
**selected_tenant** | [**IdentityApiUserV2TenantMeProfile**](IdentityApiUserV2TenantMeProfile.md) |  | [optional] 
**platform_role** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v2_user_me_profile import IdentityApiUserV2UserMeProfile

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV2UserMeProfile from a JSON string
identity_api_user_v2_user_me_profile_instance = IdentityApiUserV2UserMeProfile.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV2UserMeProfile.to_json())

# convert the object into a dict
identity_api_user_v2_user_me_profile_dict = identity_api_user_v2_user_me_profile_instance.to_dict()
# create an instance of IdentityApiUserV2UserMeProfile from a dict
identity_api_user_v2_user_me_profile_from_dict = IdentityApiUserV2UserMeProfile.from_dict(identity_api_user_v2_user_me_profile_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


