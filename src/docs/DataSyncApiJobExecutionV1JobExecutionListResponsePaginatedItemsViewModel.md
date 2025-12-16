# DataSyncApiJobExecutionV1JobExecutionListResponsePaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[DataSyncApiJobExecutionV1JobExecutionListResponse]**](DataSyncApiJobExecutionV1JobExecutionListResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_execution_v1_job_execution_list_response_paginated_items_view_model import DataSyncApiJobExecutionV1JobExecutionListResponsePaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobExecutionV1JobExecutionListResponsePaginatedItemsViewModel from a JSON string
data_sync_api_job_execution_v1_job_execution_list_response_paginated_items_view_model_instance = DataSyncApiJobExecutionV1JobExecutionListResponsePaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobExecutionV1JobExecutionListResponsePaginatedItemsViewModel.to_json())

# convert the object into a dict
data_sync_api_job_execution_v1_job_execution_list_response_paginated_items_view_model_dict = data_sync_api_job_execution_v1_job_execution_list_response_paginated_items_view_model_instance.to_dict()
# create an instance of DataSyncApiJobExecutionV1JobExecutionListResponsePaginatedItemsViewModel from a dict
data_sync_api_job_execution_v1_job_execution_list_response_paginated_items_view_model_from_dict = DataSyncApiJobExecutionV1JobExecutionListResponsePaginatedItemsViewModel.from_dict(data_sync_api_job_execution_v1_job_execution_list_response_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


