# DataSyncApiJobV1JobExecutionRequestedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_v1_job_execution_requested_response import DataSyncApiJobV1JobExecutionRequestedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobV1JobExecutionRequestedResponse from a JSON string
data_sync_api_job_v1_job_execution_requested_response_instance = DataSyncApiJobV1JobExecutionRequestedResponse.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobV1JobExecutionRequestedResponse.to_json())

# convert the object into a dict
data_sync_api_job_v1_job_execution_requested_response_dict = data_sync_api_job_v1_job_execution_requested_response_instance.to_dict()
# create an instance of DataSyncApiJobV1JobExecutionRequestedResponse from a dict
data_sync_api_job_v1_job_execution_requested_response_from_dict = DataSyncApiJobV1JobExecutionRequestedResponse.from_dict(data_sync_api_job_v1_job_execution_requested_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


