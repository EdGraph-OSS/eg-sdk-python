# DataSyncApiJobTypeV1JobTypeListResponsePaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[DataSyncApiJobTypeV1JobTypeListResponse]**](DataSyncApiJobTypeV1JobTypeListResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_type_v1_job_type_list_response_paginated_items_view_model import DataSyncApiJobTypeV1JobTypeListResponsePaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobTypeV1JobTypeListResponsePaginatedItemsViewModel from a JSON string
data_sync_api_job_type_v1_job_type_list_response_paginated_items_view_model_instance = DataSyncApiJobTypeV1JobTypeListResponsePaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobTypeV1JobTypeListResponsePaginatedItemsViewModel.to_json())

# convert the object into a dict
data_sync_api_job_type_v1_job_type_list_response_paginated_items_view_model_dict = data_sync_api_job_type_v1_job_type_list_response_paginated_items_view_model_instance.to_dict()
# create an instance of DataSyncApiJobTypeV1JobTypeListResponsePaginatedItemsViewModel from a dict
data_sync_api_job_type_v1_job_type_list_response_paginated_items_view_model_from_dict = DataSyncApiJobTypeV1JobTypeListResponsePaginatedItemsViewModel.from_dict(data_sync_api_job_type_v1_job_type_list_response_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


