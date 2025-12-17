# DataSyncApiJobV1ExecuteJobRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**child_job_id** | **str** |  | [optional] 
**data_refresh_type** | [**DataSyncApiJobV1DataRefreshType**](DataSyncApiJobV1DataRefreshType.md) |  | [optional] 
**data_refresh_specific_date** | **str** |  | [optional] 
**job_execution_metadata** | [**List[DataSyncApiJobV1JobExecutionMetadata]**](DataSyncApiJobV1JobExecutionMetadata.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_v1_execute_job_request import DataSyncApiJobV1ExecuteJobRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobV1ExecuteJobRequest from a JSON string
data_sync_api_job_v1_execute_job_request_instance = DataSyncApiJobV1ExecuteJobRequest.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobV1ExecuteJobRequest.to_json())

# convert the object into a dict
data_sync_api_job_v1_execute_job_request_dict = data_sync_api_job_v1_execute_job_request_instance.to_dict()
# create an instance of DataSyncApiJobV1ExecuteJobRequest from a dict
data_sync_api_job_v1_execute_job_request_from_dict = DataSyncApiJobV1ExecuteJobRequest.from_dict(data_sync_api_job_v1_execute_job_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


