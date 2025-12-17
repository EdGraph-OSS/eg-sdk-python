# DataSyncApiJobV1Schedule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  | [optional] 
**begin_date** | **str** |  | [optional] 
**end_date** | **str** |  | [optional] 
**cron** | **str** |  | [optional] 
**time_zone** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_v1_schedule import DataSyncApiJobV1Schedule

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobV1Schedule from a JSON string
data_sync_api_job_v1_schedule_instance = DataSyncApiJobV1Schedule.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobV1Schedule.to_json())

# convert the object into a dict
data_sync_api_job_v1_schedule_dict = data_sync_api_job_v1_schedule_instance.to_dict()
# create an instance of DataSyncApiJobV1Schedule from a dict
data_sync_api_job_v1_schedule_from_dict = DataSyncApiJobV1Schedule.from_dict(data_sync_api_job_v1_schedule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


