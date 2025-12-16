# IdentityApiInvitationV1InvitationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**invitation_id** | **str** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**role** | **str** |  | [optional] 
**invitation_token** | **str** |  | [optional] 
**invitation_status** | [**IdentityApiInvitationV1InvitationStatus**](IdentityApiInvitationV1InvitationStatus.md) |  | [optional] 
**invitation_sent_date_time** | **str** |  | [optional] 
**assign_license_requests** | [**List[IdentityApiInvitationV1AssignLicenseRequest]**](IdentityApiInvitationV1AssignLicenseRequest.md) |  | [optional] [readonly] 
**invitation_url** | **str** |  | [optional] 
**organization_name** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_invitation_v1_invitation_response import IdentityApiInvitationV1InvitationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiInvitationV1InvitationResponse from a JSON string
identity_api_invitation_v1_invitation_response_instance = IdentityApiInvitationV1InvitationResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiInvitationV1InvitationResponse.to_json())

# convert the object into a dict
identity_api_invitation_v1_invitation_response_dict = identity_api_invitation_v1_invitation_response_instance.to_dict()
# create an instance of IdentityApiInvitationV1InvitationResponse from a dict
identity_api_invitation_v1_invitation_response_from_dict = IdentityApiInvitationV1InvitationResponse.from_dict(identity_api_invitation_v1_invitation_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


