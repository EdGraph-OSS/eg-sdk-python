# DataSyncApiJobTypeV1Profile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**job_type_id** | **str** |  | [optional] 
**profile_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**actor_type** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_type_v1_profile import DataSyncApiJobTypeV1Profile

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobTypeV1Profile from a JSON string
data_sync_api_job_type_v1_profile_instance = DataSyncApiJobTypeV1Profile.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobTypeV1Profile.to_json())

# convert the object into a dict
data_sync_api_job_type_v1_profile_dict = data_sync_api_job_type_v1_profile_instance.to_dict()
# create an instance of DataSyncApiJobTypeV1Profile from a dict
data_sync_api_job_type_v1_profile_from_dict = DataSyncApiJobTypeV1Profile.from_dict(data_sync_api_job_type_v1_profile_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


