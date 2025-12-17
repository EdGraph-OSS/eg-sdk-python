# IdentityApiUserV2UserTenantProfileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**source** | **str** |  | [optional] 
**roles** | **List[str]** |  | [optional] [readonly] 
**license_count** | **int** |  | [optional] 
**organization_name** | **str** |  | [optional] 
**seoaa_count** | **int** |  | [optional] 
**section_count** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v2_user_tenant_profile_response import IdentityApiUserV2UserTenantProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV2UserTenantProfileResponse from a JSON string
identity_api_user_v2_user_tenant_profile_response_instance = IdentityApiUserV2UserTenantProfileResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV2UserTenantProfileResponse.to_json())

# convert the object into a dict
identity_api_user_v2_user_tenant_profile_response_dict = identity_api_user_v2_user_tenant_profile_response_instance.to_dict()
# create an instance of IdentityApiUserV2UserTenantProfileResponse from a dict
identity_api_user_v2_user_tenant_profile_response_from_dict = IdentityApiUserV2UserTenantProfileResponse.from_dict(identity_api_user_v2_user_tenant_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


