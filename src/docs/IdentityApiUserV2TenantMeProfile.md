# IdentityApiUserV2TenantMeProfile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**tenant_types** | **List[str]** |  | [optional] [readonly] 
**status** | **str** |  | [optional] 
**organization_identifier** | **str** |  | [optional] 
**organization_name** | **str** |  | [optional] 
**roles** | **List[str]** |  | [optional] [readonly] 
**license_count** | **int** |  | [optional] 
**seoaa_count** | **int** |  | [optional] 
**section_count** | **int** |  | [optional] 
**branding** | [**TenantApiTenantV1TenantBrandingResponse**](TenantApiTenantV1TenantBrandingResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v2_tenant_me_profile import IdentityApiUserV2TenantMeProfile

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV2TenantMeProfile from a JSON string
identity_api_user_v2_tenant_me_profile_instance = IdentityApiUserV2TenantMeProfile.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV2TenantMeProfile.to_json())

# convert the object into a dict
identity_api_user_v2_tenant_me_profile_dict = identity_api_user_v2_tenant_me_profile_instance.to_dict()
# create an instance of IdentityApiUserV2TenantMeProfile from a dict
identity_api_user_v2_tenant_me_profile_from_dict = IdentityApiUserV2TenantMeProfile.from_dict(identity_api_user_v2_tenant_me_profile_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


