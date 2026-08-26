# IdentityApiUserV1ComputedLicenseApplicationRole


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**role** | **str** |  | [optional] 
**is_assigned** | **bool** |  | [optional] 
**display_name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**sort_order** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_computed_license_application_role import IdentityApiUserV1ComputedLicenseApplicationRole

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1ComputedLicenseApplicationRole from a JSON string
identity_api_user_v1_computed_license_application_role_instance = IdentityApiUserV1ComputedLicenseApplicationRole.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1ComputedLicenseApplicationRole.to_json())

# convert the object into a dict
identity_api_user_v1_computed_license_application_role_dict = identity_api_user_v1_computed_license_application_role_instance.to_dict()
# create an instance of IdentityApiUserV1ComputedLicenseApplicationRole from a dict
identity_api_user_v1_computed_license_application_role_from_dict = IdentityApiUserV1ComputedLicenseApplicationRole.from_dict(identity_api_user_v1_computed_license_application_role_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


