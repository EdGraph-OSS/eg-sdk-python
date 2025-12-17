# DataSyncApiJobV1JobListResponsePaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[DataSyncApiJobV1JobListResponse]**](DataSyncApiJobV1JobListResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_v1_job_list_response_paginated_items_view_model import DataSyncApiJobV1JobListResponsePaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobV1JobListResponsePaginatedItemsViewModel from a JSON string
data_sync_api_job_v1_job_list_response_paginated_items_view_model_instance = DataSyncApiJobV1JobListResponsePaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobV1JobListResponsePaginatedItemsViewModel.to_json())

# convert the object into a dict
data_sync_api_job_v1_job_list_response_paginated_items_view_model_dict = data_sync_api_job_v1_job_list_response_paginated_items_view_model_instance.to_dict()
# create an instance of DataSyncApiJobV1JobListResponsePaginatedItemsViewModel from a dict
data_sync_api_job_v1_job_list_response_paginated_items_view_model_from_dict = DataSyncApiJobV1JobListResponsePaginatedItemsViewModel.from_dict(data_sync_api_job_v1_job_list_response_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


