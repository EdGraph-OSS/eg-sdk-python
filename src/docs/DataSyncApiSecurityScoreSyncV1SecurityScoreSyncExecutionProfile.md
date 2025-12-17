# DataSyncApiSecurityScoreSyncV1SecurityScoreSyncExecutionProfile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**job_status** | **str** |  | [optional] 
**job_execution_id** | **str** |  | [optional] 
**job_execution_status** | **str** |  | [optional] 
**job_execution_start_date_time** | **str** |  | [optional] 
**job_execution_end_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_security_score_sync_v1_security_score_sync_execution_profile import DataSyncApiSecurityScoreSyncV1SecurityScoreSyncExecutionProfile

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiSecurityScoreSyncV1SecurityScoreSyncExecutionProfile from a JSON string
data_sync_api_security_score_sync_v1_security_score_sync_execution_profile_instance = DataSyncApiSecurityScoreSyncV1SecurityScoreSyncExecutionProfile.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiSecurityScoreSyncV1SecurityScoreSyncExecutionProfile.to_json())

# convert the object into a dict
data_sync_api_security_score_sync_v1_security_score_sync_execution_profile_dict = data_sync_api_security_score_sync_v1_security_score_sync_execution_profile_instance.to_dict()
# create an instance of DataSyncApiSecurityScoreSyncV1SecurityScoreSyncExecutionProfile from a dict
data_sync_api_security_score_sync_v1_security_score_sync_execution_profile_from_dict = DataSyncApiSecurityScoreSyncV1SecurityScoreSyncExecutionProfile.from_dict(data_sync_api_security_score_sync_v1_security_score_sync_execution_profile_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


