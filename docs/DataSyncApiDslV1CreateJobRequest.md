# DataSyncApiDslV1CreateJobRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**dag_workflow** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**start_date** | **str** |  | [optional] 
**end_date** | **str** |  | [optional] 
**cron** | **str** |  | [optional] 
**time_zone** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_dsl_v1_create_job_request import DataSyncApiDslV1CreateJobRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiDslV1CreateJobRequest from a JSON string
data_sync_api_dsl_v1_create_job_request_instance = DataSyncApiDslV1CreateJobRequest.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiDslV1CreateJobRequest.to_json())

# convert the object into a dict
data_sync_api_dsl_v1_create_job_request_dict = data_sync_api_dsl_v1_create_job_request_instance.to_dict()
# create an instance of DataSyncApiDslV1CreateJobRequest from a dict
data_sync_api_dsl_v1_create_job_request_from_dict = DataSyncApiDslV1CreateJobRequest.from_dict(data_sync_api_dsl_v1_create_job_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


