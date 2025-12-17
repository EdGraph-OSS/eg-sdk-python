# DataSyncApiJobV1ActivateJobRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_v1_activate_job_request import DataSyncApiJobV1ActivateJobRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobV1ActivateJobRequest from a JSON string
data_sync_api_job_v1_activate_job_request_instance = DataSyncApiJobV1ActivateJobRequest.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobV1ActivateJobRequest.to_json())

# convert the object into a dict
data_sync_api_job_v1_activate_job_request_dict = data_sync_api_job_v1_activate_job_request_instance.to_dict()
# create an instance of DataSyncApiJobV1ActivateJobRequest from a dict
data_sync_api_job_v1_activate_job_request_from_dict = DataSyncApiJobV1ActivateJobRequest.from_dict(data_sync_api_job_v1_activate_job_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


