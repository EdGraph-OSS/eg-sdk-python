# IdentityApiApiClientV1ApiClientPaginatedItemsResponsePaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[IdentityApiApiClientV1ApiClientPaginatedItemsResponse]**](IdentityApiApiClientV1ApiClientPaginatedItemsResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_api_client_v1_api_client_paginated_items_response_paginated_items_view_model import IdentityApiApiClientV1ApiClientPaginatedItemsResponsePaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiApiClientV1ApiClientPaginatedItemsResponsePaginatedItemsViewModel from a JSON string
identity_api_api_client_v1_api_client_paginated_items_response_paginated_items_view_model_instance = IdentityApiApiClientV1ApiClientPaginatedItemsResponsePaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(IdentityApiApiClientV1ApiClientPaginatedItemsResponsePaginatedItemsViewModel.to_json())

# convert the object into a dict
identity_api_api_client_v1_api_client_paginated_items_response_paginated_items_view_model_dict = identity_api_api_client_v1_api_client_paginated_items_response_paginated_items_view_model_instance.to_dict()
# create an instance of IdentityApiApiClientV1ApiClientPaginatedItemsResponsePaginatedItemsViewModel from a dict
identity_api_api_client_v1_api_client_paginated_items_response_paginated_items_view_model_from_dict = IdentityApiApiClientV1ApiClientPaginatedItemsResponsePaginatedItemsViewModel.from_dict(identity_api_api_client_v1_api_client_paginated_items_response_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


