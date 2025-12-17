# DataSyncApiProviderV1ProviderProfileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**provider_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**icon_uri** | **str** |  | [optional] 
**connection_types** | [**List[DataSyncApiProviderV1ConnectionType]**](DataSyncApiProviderV1ConnectionType.md) |  | [optional] [readonly] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_provider_v1_provider_profile_response import DataSyncApiProviderV1ProviderProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiProviderV1ProviderProfileResponse from a JSON string
data_sync_api_provider_v1_provider_profile_response_instance = DataSyncApiProviderV1ProviderProfileResponse.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiProviderV1ProviderProfileResponse.to_json())

# convert the object into a dict
data_sync_api_provider_v1_provider_profile_response_dict = data_sync_api_provider_v1_provider_profile_response_instance.to_dict()
# create an instance of DataSyncApiProviderV1ProviderProfileResponse from a dict
data_sync_api_provider_v1_provider_profile_response_from_dict = DataSyncApiProviderV1ProviderProfileResponse.from_dict(data_sync_api_provider_v1_provider_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


