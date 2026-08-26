# IdentityApiUserV2UserProfileResponse

Entities

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**user_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**phone_number** | **str** |  | [optional] 
**lockout_enabled** | **bool** |  | [optional] 
**tenant_count** | **int** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**extensions** | [**List[IdentityApiUserV2UserExtension]**](IdentityApiUserV2UserExtension.md) |  | [optional] [readonly] 
**logins** | [**List[IdentityApiUserV2UserLogin]**](IdentityApiUserV2UserLogin.md) |  | [optional] [readonly] 
**source** | **str** |  | [optional] 
**last_login_date_time** | **str** |  | [optional] 
**mfa_completed** | **bool** |  | [optional] 
**platform_role** | **str** |  | [optional] 
**tenant_status** | **str** |  | [optional] 
**tenant_admin** | **bool** |  | [optional] 
**status** | **str** | The user&#39;s status across all their tenants: Active if any membership is active, Inactive if every  membership is inactive, Unknown if they have no memberships. Unlike tenantStatus this does not  depend on a tenantId being supplied on the request. | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v2_user_profile_response import IdentityApiUserV2UserProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV2UserProfileResponse from a JSON string
identity_api_user_v2_user_profile_response_instance = IdentityApiUserV2UserProfileResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV2UserProfileResponse.to_json())

# convert the object into a dict
identity_api_user_v2_user_profile_response_dict = identity_api_user_v2_user_profile_response_instance.to_dict()
# create an instance of IdentityApiUserV2UserProfileResponse from a dict
identity_api_user_v2_user_profile_response_from_dict = IdentityApiUserV2UserProfileResponse.from_dict(identity_api_user_v2_user_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


