# IdentityApiUserV1UserTenantProfileTypesUserTenantEducationOrganizationProfile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**education_organization_id** | **int** |  | [optional] 
**short_name_of_institution** | **str** |  | [optional] 
**name_of_institution** | **str** |  | [optional] 
**staff_classifications** | **List[str]** |  | [optional] [readonly] 
**source** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_user_tenant_profile_types_user_tenant_education_organization_profile import IdentityApiUserV1UserTenantProfileTypesUserTenantEducationOrganizationProfile

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1UserTenantProfileTypesUserTenantEducationOrganizationProfile from a JSON string
identity_api_user_v1_user_tenant_profile_types_user_tenant_education_organization_profile_instance = IdentityApiUserV1UserTenantProfileTypesUserTenantEducationOrganizationProfile.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1UserTenantProfileTypesUserTenantEducationOrganizationProfile.to_json())

# convert the object into a dict
identity_api_user_v1_user_tenant_profile_types_user_tenant_education_organization_profile_dict = identity_api_user_v1_user_tenant_profile_types_user_tenant_education_organization_profile_instance.to_dict()
# create an instance of IdentityApiUserV1UserTenantProfileTypesUserTenantEducationOrganizationProfile from a dict
identity_api_user_v1_user_tenant_profile_types_user_tenant_education_organization_profile_from_dict = IdentityApiUserV1UserTenantProfileTypesUserTenantEducationOrganizationProfile.from_dict(identity_api_user_v1_user_tenant_profile_types_user_tenant_education_organization_profile_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


