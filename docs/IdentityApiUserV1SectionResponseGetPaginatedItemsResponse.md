# IdentityApiUserV1SectionResponseGetPaginatedItemsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**data** | [**List[IdentityApiUserV1SectionResponse]**](IdentityApiUserV1SectionResponse.md) |  | [optional] 
**count** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_section_response_get_paginated_items_response import IdentityApiUserV1SectionResponseGetPaginatedItemsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1SectionResponseGetPaginatedItemsResponse from a JSON string
identity_api_user_v1_section_response_get_paginated_items_response_instance = IdentityApiUserV1SectionResponseGetPaginatedItemsResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1SectionResponseGetPaginatedItemsResponse.to_json())

# convert the object into a dict
identity_api_user_v1_section_response_get_paginated_items_response_dict = identity_api_user_v1_section_response_get_paginated_items_response_instance.to_dict()
# create an instance of IdentityApiUserV1SectionResponseGetPaginatedItemsResponse from a dict
identity_api_user_v1_section_response_get_paginated_items_response_from_dict = IdentityApiUserV1SectionResponseGetPaginatedItemsResponse.from_dict(identity_api_user_v1_section_response_get_paginated_items_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


