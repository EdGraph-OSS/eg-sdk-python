# IdentityApiInvitationV1InvitationListResponsePaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[IdentityApiInvitationV1InvitationListResponse]**](IdentityApiInvitationV1InvitationListResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_invitation_v1_invitation_list_response_paginated_items_view_model import IdentityApiInvitationV1InvitationListResponsePaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiInvitationV1InvitationListResponsePaginatedItemsViewModel from a JSON string
identity_api_invitation_v1_invitation_list_response_paginated_items_view_model_instance = IdentityApiInvitationV1InvitationListResponsePaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(IdentityApiInvitationV1InvitationListResponsePaginatedItemsViewModel.to_json())

# convert the object into a dict
identity_api_invitation_v1_invitation_list_response_paginated_items_view_model_dict = identity_api_invitation_v1_invitation_list_response_paginated_items_view_model_instance.to_dict()
# create an instance of IdentityApiInvitationV1InvitationListResponsePaginatedItemsViewModel from a dict
identity_api_invitation_v1_invitation_list_response_paginated_items_view_model_from_dict = IdentityApiInvitationV1InvitationListResponsePaginatedItemsViewModel.from_dict(identity_api_invitation_v1_invitation_list_response_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


