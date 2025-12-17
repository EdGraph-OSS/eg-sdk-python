# DataSyncApiJobExecutionLogV1JobExecutionLogEntryPaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[DataSyncApiJobExecutionLogV1JobExecutionLogEntry]**](DataSyncApiJobExecutionLogV1JobExecutionLogEntry.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_execution_log_v1_job_execution_log_entry_paginated_items_view_model import DataSyncApiJobExecutionLogV1JobExecutionLogEntryPaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobExecutionLogV1JobExecutionLogEntryPaginatedItemsViewModel from a JSON string
data_sync_api_job_execution_log_v1_job_execution_log_entry_paginated_items_view_model_instance = DataSyncApiJobExecutionLogV1JobExecutionLogEntryPaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobExecutionLogV1JobExecutionLogEntryPaginatedItemsViewModel.to_json())

# convert the object into a dict
data_sync_api_job_execution_log_v1_job_execution_log_entry_paginated_items_view_model_dict = data_sync_api_job_execution_log_v1_job_execution_log_entry_paginated_items_view_model_instance.to_dict()
# create an instance of DataSyncApiJobExecutionLogV1JobExecutionLogEntryPaginatedItemsViewModel from a dict
data_sync_api_job_execution_log_v1_job_execution_log_entry_paginated_items_view_model_from_dict = DataSyncApiJobExecutionLogV1JobExecutionLogEntryPaginatedItemsViewModel.from_dict(data_sync_api_job_execution_log_v1_job_execution_log_entry_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


