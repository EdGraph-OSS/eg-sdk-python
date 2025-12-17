# IdentityApiUserV1RevokeLicenseRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**subscription_id** | **str** |  | [optional] 
**application_id** | **str** |  | [optional] 
**user_id** | **str** |  | [optional] 
**strategy** | [**IdentityApiUserV1RevokeStrategy**](IdentityApiUserV1RevokeStrategy.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_revoke_license_request import IdentityApiUserV1RevokeLicenseRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1RevokeLicenseRequest from a JSON string
identity_api_user_v1_revoke_license_request_instance = IdentityApiUserV1RevokeLicenseRequest.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1RevokeLicenseRequest.to_json())

# convert the object into a dict
identity_api_user_v1_revoke_license_request_dict = identity_api_user_v1_revoke_license_request_instance.to_dict()
# create an instance of IdentityApiUserV1RevokeLicenseRequest from a dict
identity_api_user_v1_revoke_license_request_from_dict = IdentityApiUserV1RevokeLicenseRequest.from_dict(identity_api_user_v1_revoke_license_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


