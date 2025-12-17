# DataSyncApiJobExecutionLogV1JobExecutionLogEntry


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**job_execution_id** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**message_type** | [**DataSyncApiJobExecutionLogV1MessageType**](DataSyncApiJobExecutionLogV1MessageType.md) |  | [optional] 
**logged_date_time** | **str** |  | [optional] 
**error_code** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_execution_log_v1_job_execution_log_entry import DataSyncApiJobExecutionLogV1JobExecutionLogEntry

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobExecutionLogV1JobExecutionLogEntry from a JSON string
data_sync_api_job_execution_log_v1_job_execution_log_entry_instance = DataSyncApiJobExecutionLogV1JobExecutionLogEntry.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobExecutionLogV1JobExecutionLogEntry.to_json())

# convert the object into a dict
data_sync_api_job_execution_log_v1_job_execution_log_entry_dict = data_sync_api_job_execution_log_v1_job_execution_log_entry_instance.to_dict()
# create an instance of DataSyncApiJobExecutionLogV1JobExecutionLogEntry from a dict
data_sync_api_job_execution_log_v1_job_execution_log_entry_from_dict = DataSyncApiJobExecutionLogV1JobExecutionLogEntry.from_dict(data_sync_api_job_execution_log_v1_job_execution_log_entry_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


