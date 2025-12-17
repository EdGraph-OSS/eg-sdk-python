# DataSyncApiJobV1ChildJob


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**job_id** | **str** |  | [optional] 
**job_execution_id** | **str** |  | [optional] 
**child_job_id** | **str** |  | [optional] 
**child_job_name** | **str** |  | [optional] 
**job_execution_status** | [**DataSyncApiJobV1JobExecutionStatus**](DataSyncApiJobV1JobExecutionStatus.md) |  | [optional] 
**job_execution_start_date_time** | **str** |  | [optional] 
**job_execution_end_date_time** | **str** |  | [optional] 
**metrics** | [**List[DataSyncApiJobV1Metric]**](DataSyncApiJobV1Metric.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_v1_child_job import DataSyncApiJobV1ChildJob

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobV1ChildJob from a JSON string
data_sync_api_job_v1_child_job_instance = DataSyncApiJobV1ChildJob.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobV1ChildJob.to_json())

# convert the object into a dict
data_sync_api_job_v1_child_job_dict = data_sync_api_job_v1_child_job_instance.to_dict()
# create an instance of DataSyncApiJobV1ChildJob from a dict
data_sync_api_job_v1_child_job_from_dict = DataSyncApiJobV1ChildJob.from_dict(data_sync_api_job_v1_child_job_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


