# DataSyncApiSecurityScoreSyncV1SecurityScoreSyncProfile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_security_score_sync_v1_security_score_sync_profile import DataSyncApiSecurityScoreSyncV1SecurityScoreSyncProfile

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiSecurityScoreSyncV1SecurityScoreSyncProfile from a JSON string
data_sync_api_security_score_sync_v1_security_score_sync_profile_instance = DataSyncApiSecurityScoreSyncV1SecurityScoreSyncProfile.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiSecurityScoreSyncV1SecurityScoreSyncProfile.to_json())

# convert the object into a dict
data_sync_api_security_score_sync_v1_security_score_sync_profile_dict = data_sync_api_security_score_sync_v1_security_score_sync_profile_instance.to_dict()
# create an instance of DataSyncApiSecurityScoreSyncV1SecurityScoreSyncProfile from a dict
data_sync_api_security_score_sync_v1_security_score_sync_profile_from_dict = DataSyncApiSecurityScoreSyncV1SecurityScoreSyncProfile.from_dict(data_sync_api_security_score_sync_v1_security_score_sync_profile_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


