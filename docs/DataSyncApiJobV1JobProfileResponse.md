# DataSyncApiJobV1JobProfileResponse


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
**profile_name** | **str** |  | [optional] 
**application_id** | **str** |  | [optional] 
**job_points** | **int** |  | [optional] 
**data_refresh_type** | [**DataSyncApiJobV1DataRefreshType**](DataSyncApiJobV1DataRefreshType.md) |  | [optional] 
**data_refresh_specific_date** | **str** |  | [optional] 
**max_api_failure** | **int** |  | [optional] 
**max_api_retry** | **int** |  | [optional] 
**job_complete_callback_url** | **str** |  | [optional] 
**job_metadata** | [**List[DataSyncApiJobV1JobMetadata]**](DataSyncApiJobV1JobMetadata.md) |  | [optional] [readonly] 
**schedule** | [**DataSyncApiJobV1Schedule**](DataSyncApiJobV1Schedule.md) |  | [optional] 
**notification_emails** | **List[str]** |  | [optional] [readonly] 
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

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_v1_job_profile_response import DataSyncApiJobV1JobProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobV1JobProfileResponse from a JSON string
data_sync_api_job_v1_job_profile_response_instance = DataSyncApiJobV1JobProfileResponse.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobV1JobProfileResponse.to_json())

# convert the object into a dict
data_sync_api_job_v1_job_profile_response_dict = data_sync_api_job_v1_job_profile_response_instance.to_dict()
# create an instance of DataSyncApiJobV1JobProfileResponse from a dict
data_sync_api_job_v1_job_profile_response_from_dict = DataSyncApiJobV1JobProfileResponse.from_dict(data_sync_api_job_v1_job_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


