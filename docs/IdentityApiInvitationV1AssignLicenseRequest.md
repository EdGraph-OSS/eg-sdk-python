# IdentityApiInvitationV1AssignLicenseRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**subscription_id** | **str** |  | [optional] 
**application_id** | **str** |  | [optional] 
**user_id** | **str** |  | [optional] 
**roles** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_invitation_v1_assign_license_request import IdentityApiInvitationV1AssignLicenseRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiInvitationV1AssignLicenseRequest from a JSON string
identity_api_invitation_v1_assign_license_request_instance = IdentityApiInvitationV1AssignLicenseRequest.from_json(json)
# print the JSON string representation of the object
print(IdentityApiInvitationV1AssignLicenseRequest.to_json())

# convert the object into a dict
identity_api_invitation_v1_assign_license_request_dict = identity_api_invitation_v1_assign_license_request_instance.to_dict()
# create an instance of IdentityApiInvitationV1AssignLicenseRequest from a dict
identity_api_invitation_v1_assign_license_request_from_dict = IdentityApiInvitationV1AssignLicenseRequest.from_dict(identity_api_invitation_v1_assign_license_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


