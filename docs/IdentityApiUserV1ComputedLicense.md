# IdentityApiUserV1ComputedLicense


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**application_id** | **str** |  | [optional] 
**application_name** | **str** |  | [optional] 
**application_role** | [**List[IdentityApiUserV1ComputedLicenseApplicationRole]**](IdentityApiUserV1ComputedLicenseApplicationRole.md) |  | [optional] [readonly] 
**application_tenant_id** | **str** |  | [optional] 
**assigned_licenses** | **int** |  | [optional] 
**is_tenant_subscribed** | **bool** |  | [optional] 
**is_user_licensed** | **bool** |  | [optional] 
**number_of_licenses** | **int** |  | [optional] 
**subscription_tenant_id** | **str** |  | [optional] 
**tenant_subscription_actual_end_date_time** | **str** |  | [optional] 
**tenant_subscription_end_date_time** | **str** |  | [optional] 
**tenant_subscription_id** | **str** |  | [optional] 
**tenant_subscription_start_date_time** | **str** |  | [optional] 
**deleted_at** | **str** |  | [optional] 
**status** | [**IdentityApiUserV1LicenseStatus**](IdentityApiUserV1LicenseStatus.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_computed_license import IdentityApiUserV1ComputedLicense

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1ComputedLicense from a JSON string
identity_api_user_v1_computed_license_instance = IdentityApiUserV1ComputedLicense.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1ComputedLicense.to_json())

# convert the object into a dict
identity_api_user_v1_computed_license_dict = identity_api_user_v1_computed_license_instance.to_dict()
# create an instance of IdentityApiUserV1ComputedLicense from a dict
identity_api_user_v1_computed_license_from_dict = IdentityApiUserV1ComputedLicense.from_dict(identity_api_user_v1_computed_license_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


