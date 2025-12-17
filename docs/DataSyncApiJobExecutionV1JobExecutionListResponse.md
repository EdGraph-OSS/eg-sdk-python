# DataSyncApiJobExecutionV1JobExecutionListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**application_id** | **str** |  | [optional] 
**job_execution_id** | **str** |  | [optional] 
**job_execution_status** | [**DataSyncApiJobExecutionV1JobExecutionStatus**](DataSyncApiJobExecutionV1JobExecutionStatus.md) |  | [optional] 
**job_execution_start_date_time** | **str** |  | [optional] 
**job_execution_end_date_time** | **str** |  | [optional] 
**child_jobs** | [**List[DataSyncApiJobExecutionV1ChildJob]**](DataSyncApiJobExecutionV1ChildJob.md) |  | [optional] [readonly] 
**metrics** | [**List[DataSyncApiJobExecutionV1Metric]**](DataSyncApiJobExecutionV1Metric.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_execution_v1_job_execution_list_response import DataSyncApiJobExecutionV1JobExecutionListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobExecutionV1JobExecutionListResponse from a JSON string
data_sync_api_job_execution_v1_job_execution_list_response_instance = DataSyncApiJobExecutionV1JobExecutionListResponse.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobExecutionV1JobExecutionListResponse.to_json())

# convert the object into a dict
data_sync_api_job_execution_v1_job_execution_list_response_dict = data_sync_api_job_execution_v1_job_execution_list_response_instance.to_dict()
# create an instance of DataSyncApiJobExecutionV1JobExecutionListResponse from a dict
data_sync_api_job_execution_v1_job_execution_list_response_from_dict = DataSyncApiJobExecutionV1JobExecutionListResponse.from_dict(data_sync_api_job_execution_v1_job_execution_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


