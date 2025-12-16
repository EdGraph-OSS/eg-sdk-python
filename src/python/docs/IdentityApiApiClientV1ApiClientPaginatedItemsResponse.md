# IdentityApiApiClientV1ApiClientPaginatedItemsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[IdentityApiApiClientV1ApiClientListResponse]**](IdentityApiApiClientV1ApiClientListResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_api_client_v1_api_client_paginated_items_response import IdentityApiApiClientV1ApiClientPaginatedItemsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiApiClientV1ApiClientPaginatedItemsResponse from a JSON string
identity_api_api_client_v1_api_client_paginated_items_response_instance = IdentityApiApiClientV1ApiClientPaginatedItemsResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiApiClientV1ApiClientPaginatedItemsResponse.to_json())

# convert the object into a dict
identity_api_api_client_v1_api_client_paginated_items_response_dict = identity_api_api_client_v1_api_client_paginated_items_response_instance.to_dict()
# create an instance of IdentityApiApiClientV1ApiClientPaginatedItemsResponse from a dict
identity_api_api_client_v1_api_client_paginated_items_response_from_dict = IdentityApiApiClientV1ApiClientPaginatedItemsResponse.from_dict(identity_api_api_client_v1_api_client_paginated_items_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


