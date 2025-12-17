# IdentityApiUserV2UsersSearchResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_size** | **int** |  | [optional] 
**page_index** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[IdentityApiUserV2UserProfileResponse]**](IdentityApiUserV2UserProfileResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v2_users_search_response import IdentityApiUserV2UsersSearchResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV2UsersSearchResponse from a JSON string
identity_api_user_v2_users_search_response_instance = IdentityApiUserV2UsersSearchResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV2UsersSearchResponse.to_json())

# convert the object into a dict
identity_api_user_v2_users_search_response_dict = identity_api_user_v2_users_search_response_instance.to_dict()
# create an instance of IdentityApiUserV2UsersSearchResponse from a dict
identity_api_user_v2_users_search_response_from_dict = IdentityApiUserV2UsersSearchResponse.from_dict(identity_api_user_v2_users_search_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


