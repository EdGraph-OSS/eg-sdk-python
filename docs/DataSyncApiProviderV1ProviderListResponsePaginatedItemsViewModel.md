# DataSyncApiProviderV1ProviderListResponsePaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[DataSyncApiProviderV1ProviderListResponse]**](DataSyncApiProviderV1ProviderListResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_provider_v1_provider_list_response_paginated_items_view_model import DataSyncApiProviderV1ProviderListResponsePaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiProviderV1ProviderListResponsePaginatedItemsViewModel from a JSON string
data_sync_api_provider_v1_provider_list_response_paginated_items_view_model_instance = DataSyncApiProviderV1ProviderListResponsePaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiProviderV1ProviderListResponsePaginatedItemsViewModel.to_json())

# convert the object into a dict
data_sync_api_provider_v1_provider_list_response_paginated_items_view_model_dict = data_sync_api_provider_v1_provider_list_response_paginated_items_view_model_instance.to_dict()
# create an instance of DataSyncApiProviderV1ProviderListResponsePaginatedItemsViewModel from a dict
data_sync_api_provider_v1_provider_list_response_paginated_items_view_model_from_dict = DataSyncApiProviderV1ProviderListResponsePaginatedItemsViewModel.from_dict(data_sync_api_provider_v1_provider_list_response_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


