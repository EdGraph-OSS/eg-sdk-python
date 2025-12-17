# DataSyncApiConnectionV1ConnectionListResponsePaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[DataSyncApiConnectionV1ConnectionListResponse]**](DataSyncApiConnectionV1ConnectionListResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_connection_v1_connection_list_response_paginated_items_view_model import DataSyncApiConnectionV1ConnectionListResponsePaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiConnectionV1ConnectionListResponsePaginatedItemsViewModel from a JSON string
data_sync_api_connection_v1_connection_list_response_paginated_items_view_model_instance = DataSyncApiConnectionV1ConnectionListResponsePaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiConnectionV1ConnectionListResponsePaginatedItemsViewModel.to_json())

# convert the object into a dict
data_sync_api_connection_v1_connection_list_response_paginated_items_view_model_dict = data_sync_api_connection_v1_connection_list_response_paginated_items_view_model_instance.to_dict()
# create an instance of DataSyncApiConnectionV1ConnectionListResponsePaginatedItemsViewModel from a dict
data_sync_api_connection_v1_connection_list_response_paginated_items_view_model_from_dict = DataSyncApiConnectionV1ConnectionListResponsePaginatedItemsViewModel.from_dict(data_sync_api_connection_v1_connection_list_response_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


