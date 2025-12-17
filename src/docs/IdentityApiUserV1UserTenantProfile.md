# IdentityApiUserV1UserTenantProfile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**tenant_types** | [**List[IdentityApiUserV1TenantType]**](IdentityApiUserV1TenantType.md) |  | [optional] [readonly] 
**tenant_status** | [**IdentityApiUserV1TenantStatus**](IdentityApiUserV1TenantStatus.md) |  | [optional] 
**organization_identifier** | **str** |  | [optional] 
**organization_name** | **str** |  | [optional] 
**state** | **str** |  | [optional] 
**is_demo** | **bool** |  | [optional] 
**education_organizations** | [**List[IdentityApiUserV1UserTenantProfileTypesUserTenantEducationOrganizationProfile]**](IdentityApiUserV1UserTenantProfileTypesUserTenantEducationOrganizationProfile.md) |  | [optional] [readonly] 
**licenses** | [**List[IdentityApiUserV1UserTenantProfileTypesUserTenantLicenseProfile]**](IdentityApiUserV1UserTenantProfileTypesUserTenantLicenseProfile.md) |  | [optional] [readonly] 
**mfa_completed** | **bool** |  | [optional] 
**tenant_type** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_user_tenant_profile import IdentityApiUserV1UserTenantProfile

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1UserTenantProfile from a JSON string
identity_api_user_v1_user_tenant_profile_instance = IdentityApiUserV1UserTenantProfile.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1UserTenantProfile.to_json())

# convert the object into a dict
identity_api_user_v1_user_tenant_profile_dict = identity_api_user_v1_user_tenant_profile_instance.to_dict()
# create an instance of IdentityApiUserV1UserTenantProfile from a dict
identity_api_user_v1_user_tenant_profile_from_dict = IdentityApiUserV1UserTenantProfile.from_dict(identity_api_user_v1_user_tenant_profile_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


