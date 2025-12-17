# IdentityApiUserV1UserTenantProfileTypesUserTenantLicenseProfile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**application_id** | **str** |  | [optional] 
**application_name** | **str** |  | [optional] 
**start_date_time** | **str** |  | [optional] 
**end_date_time** | **str** |  | [optional] 
**roles** | [**List[IdentityApiUserV1UserTenantProfileTypesUserTenantLicenseProfileTypesUserTenantLicenseRoleProfile]**](IdentityApiUserV1UserTenantProfileTypesUserTenantLicenseProfileTypesUserTenantLicenseRoleProfile.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_user_tenant_profile_types_user_tenant_license_profile import IdentityApiUserV1UserTenantProfileTypesUserTenantLicenseProfile

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1UserTenantProfileTypesUserTenantLicenseProfile from a JSON string
identity_api_user_v1_user_tenant_profile_types_user_tenant_license_profile_instance = IdentityApiUserV1UserTenantProfileTypesUserTenantLicenseProfile.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1UserTenantProfileTypesUserTenantLicenseProfile.to_json())

# convert the object into a dict
identity_api_user_v1_user_tenant_profile_types_user_tenant_license_profile_dict = identity_api_user_v1_user_tenant_profile_types_user_tenant_license_profile_instance.to_dict()
# create an instance of IdentityApiUserV1UserTenantProfileTypesUserTenantLicenseProfile from a dict
identity_api_user_v1_user_tenant_profile_types_user_tenant_license_profile_from_dict = IdentityApiUserV1UserTenantProfileTypesUserTenantLicenseProfile.from_dict(identity_api_user_v1_user_tenant_profile_types_user_tenant_license_profile_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


