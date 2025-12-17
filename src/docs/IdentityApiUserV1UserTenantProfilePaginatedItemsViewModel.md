# IdentityApiUserV1UserTenantProfilePaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[IdentityApiUserV1UserTenantProfile]**](IdentityApiUserV1UserTenantProfile.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_user_tenant_profile_paginated_items_view_model import IdentityApiUserV1UserTenantProfilePaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1UserTenantProfilePaginatedItemsViewModel from a JSON string
identity_api_user_v1_user_tenant_profile_paginated_items_view_model_instance = IdentityApiUserV1UserTenantProfilePaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1UserTenantProfilePaginatedItemsViewModel.to_json())

# convert the object into a dict
identity_api_user_v1_user_tenant_profile_paginated_items_view_model_dict = identity_api_user_v1_user_tenant_profile_paginated_items_view_model_instance.to_dict()
# create an instance of IdentityApiUserV1UserTenantProfilePaginatedItemsViewModel from a dict
identity_api_user_v1_user_tenant_profile_paginated_items_view_model_from_dict = IdentityApiUserV1UserTenantProfilePaginatedItemsViewModel.from_dict(identity_api_user_v1_user_tenant_profile_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


