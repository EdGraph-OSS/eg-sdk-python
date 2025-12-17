# DataSyncApiJobV1CancelJobRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**child_job_id** | **str** |  | [optional] 
**job_execution_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_v1_cancel_job_request import DataSyncApiJobV1CancelJobRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobV1CancelJobRequest from a JSON string
data_sync_api_job_v1_cancel_job_request_instance = DataSyncApiJobV1CancelJobRequest.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobV1CancelJobRequest.to_json())

# convert the object into a dict
data_sync_api_job_v1_cancel_job_request_dict = data_sync_api_job_v1_cancel_job_request_instance.to_dict()
# create an instance of DataSyncApiJobV1CancelJobRequest from a dict
data_sync_api_job_v1_cancel_job_request_from_dict = DataSyncApiJobV1CancelJobRequest.from_dict(data_sync_api_job_v1_cancel_job_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


