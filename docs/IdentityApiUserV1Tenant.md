# IdentityApiUserV1Tenant


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**status** | [**IdentityApiUserV1TenantStatus**](IdentityApiUserV1TenantStatus.md) |  | [optional] 
**source** | [**IdentityApiUserV1TenantSource**](IdentityApiUserV1TenantSource.md) |  | [optional] 
**roles** | **List[str]** |  | [optional] [readonly] 
**education_organizations** | [**List[IdentityApiUserV1EducationOrganization]**](IdentityApiUserV1EducationOrganization.md) |  | [optional] [readonly] 
**licenses** | [**List[IdentityApiUserV1ComputedLicense]**](IdentityApiUserV1ComputedLicense.md) |  | [optional] [readonly] 
**organization_name** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_tenant import IdentityApiUserV1Tenant

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1Tenant from a JSON string
identity_api_user_v1_tenant_instance = IdentityApiUserV1Tenant.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1Tenant.to_json())

# convert the object into a dict
identity_api_user_v1_tenant_dict = identity_api_user_v1_tenant_instance.to_dict()
# create an instance of IdentityApiUserV1Tenant from a dict
identity_api_user_v1_tenant_from_dict = IdentityApiUserV1Tenant.from_dict(identity_api_user_v1_tenant_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


