# IdentityApiUserV1UserTenantStatusProfile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | [optional] 
**username** | **str** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**platform_role** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_user_tenant_status_profile import IdentityApiUserV1UserTenantStatusProfile

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1UserTenantStatusProfile from a JSON string
identity_api_user_v1_user_tenant_status_profile_instance = IdentityApiUserV1UserTenantStatusProfile.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1UserTenantStatusProfile.to_json())

# convert the object into a dict
identity_api_user_v1_user_tenant_status_profile_dict = identity_api_user_v1_user_tenant_status_profile_instance.to_dict()
# create an instance of IdentityApiUserV1UserTenantStatusProfile from a dict
identity_api_user_v1_user_tenant_status_profile_from_dict = IdentityApiUserV1UserTenantStatusProfile.from_dict(identity_api_user_v1_user_tenant_status_profile_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


