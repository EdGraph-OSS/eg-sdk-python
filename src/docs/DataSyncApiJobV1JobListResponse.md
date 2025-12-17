# DataSyncApiJobV1JobListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**job_type_id** | **str** |  | [optional] 
**job_type_name** | **str** |  | [optional] 
**source_connection_id** | **str** |  | [optional] 
**destination_connection_id** | **str** |  | [optional] 
**profile_id** | **str** |  | [optional] 
**application_id** | **str** |  | [optional] 
**schedule** | [**DataSyncApiJobV1Schedule**](DataSyncApiJobV1Schedule.md) |  | [optional] 
**job_status** | [**DataSyncApiJobV1JobStatus**](DataSyncApiJobV1JobStatus.md) |  | [optional] 
**job_execution_id** | **str** |  | [optional] 
**job_execution_status** | [**DataSyncApiJobV1JobExecutionStatus**](DataSyncApiJobV1JobExecutionStatus.md) |  | [optional] 
**job_execution_start_date_time** | **str** |  | [optional] 
**job_execution_end_date_time** | **str** |  | [optional] 
**metrics** | [**List[DataSyncApiJobV1Metric]**](DataSyncApiJobV1Metric.md) |  | [optional] [readonly] 
**child_jobs** | [**List[DataSyncApiJobV1ChildJob]**](DataSyncApiJobV1ChildJob.md) |  | [optional] [readonly] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**job_execution_queued_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_v1_job_list_response import DataSyncApiJobV1JobListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobV1JobListResponse from a JSON string
data_sync_api_job_v1_job_list_response_instance = DataSyncApiJobV1JobListResponse.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobV1JobListResponse.to_json())

# convert the object into a dict
data_sync_api_job_v1_job_list_response_dict = data_sync_api_job_v1_job_list_response_instance.to_dict()
# create an instance of DataSyncApiJobV1JobListResponse from a dict
data_sync_api_job_v1_job_list_response_from_dict = DataSyncApiJobV1JobListResponse.from_dict(data_sync_api_job_v1_job_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


