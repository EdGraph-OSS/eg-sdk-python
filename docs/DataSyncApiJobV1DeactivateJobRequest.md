# DataSyncApiJobV1DeactivateJobRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_v1_deactivate_job_request import DataSyncApiJobV1DeactivateJobRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobV1DeactivateJobRequest from a JSON string
data_sync_api_job_v1_deactivate_job_request_instance = DataSyncApiJobV1DeactivateJobRequest.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobV1DeactivateJobRequest.to_json())

# convert the object into a dict
data_sync_api_job_v1_deactivate_job_request_dict = data_sync_api_job_v1_deactivate_job_request_instance.to_dict()
# create an instance of DataSyncApiJobV1DeactivateJobRequest from a dict
data_sync_api_job_v1_deactivate_job_request_from_dict = DataSyncApiJobV1DeactivateJobRequest.from_dict(data_sync_api_job_v1_deactivate_job_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


