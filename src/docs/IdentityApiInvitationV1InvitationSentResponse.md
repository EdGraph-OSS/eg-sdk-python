# IdentityApiInvitationV1InvitationSentResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**invitation_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_invitation_v1_invitation_sent_response import IdentityApiInvitationV1InvitationSentResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiInvitationV1InvitationSentResponse from a JSON string
identity_api_invitation_v1_invitation_sent_response_instance = IdentityApiInvitationV1InvitationSentResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiInvitationV1InvitationSentResponse.to_json())

# convert the object into a dict
identity_api_invitation_v1_invitation_sent_response_dict = identity_api_invitation_v1_invitation_sent_response_instance.to_dict()
# create an instance of IdentityApiInvitationV1InvitationSentResponse from a dict
identity_api_invitation_v1_invitation_sent_response_from_dict = IdentityApiInvitationV1InvitationSentResponse.from_dict(identity_api_invitation_v1_invitation_sent_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


