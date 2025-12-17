# IdentityApiUserV2UserLicenseProfileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**application_id** | **str** |  | [optional] 
**application_name** | **str** |  | [optional] 
**role** | [**IdentityApiUserV2UserLicenseRole**](IdentityApiUserV2UserLicenseRole.md) |  | [optional] 
**license_status** | **str** |  | [optional] 
**license_source** | **str** |  | [optional] 
**education_organization_id** | **int** |  | [optional] 
**education_organization_source** | **str** |  | [optional] 
**staff_classification** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v2_user_license_profile_response import IdentityApiUserV2UserLicenseProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV2UserLicenseProfileResponse from a JSON string
identity_api_user_v2_user_license_profile_response_instance = IdentityApiUserV2UserLicenseProfileResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV2UserLicenseProfileResponse.to_json())

# convert the object into a dict
identity_api_user_v2_user_license_profile_response_dict = identity_api_user_v2_user_license_profile_response_instance.to_dict()
# create an instance of IdentityApiUserV2UserLicenseProfileResponse from a dict
identity_api_user_v2_user_license_profile_response_from_dict = IdentityApiUserV2UserLicenseProfileResponse.from_dict(identity_api_user_v2_user_license_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


