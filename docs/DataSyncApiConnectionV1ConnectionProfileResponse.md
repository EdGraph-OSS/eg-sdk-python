# DataSyncApiConnectionV1ConnectionProfileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**connection_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**connection_metadata** | [**List[DataSyncApiConnectionV1ConnectionMetadata]**](DataSyncApiConnectionV1ConnectionMetadata.md) |  | [optional] [readonly] 
**provider_id** | **str** |  | [optional] 
**provider_name** | **str** |  | [optional] 
**connection_type_id** | **str** |  | [optional] 
**connection_type_name** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_connection_v1_connection_profile_response import DataSyncApiConnectionV1ConnectionProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiConnectionV1ConnectionProfileResponse from a JSON string
data_sync_api_connection_v1_connection_profile_response_instance = DataSyncApiConnectionV1ConnectionProfileResponse.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiConnectionV1ConnectionProfileResponse.to_json())

# convert the object into a dict
data_sync_api_connection_v1_connection_profile_response_dict = data_sync_api_connection_v1_connection_profile_response_instance.to_dict()
# create an instance of DataSyncApiConnectionV1ConnectionProfileResponse from a dict
data_sync_api_connection_v1_connection_profile_response_from_dict = DataSyncApiConnectionV1ConnectionProfileResponse.from_dict(data_sync_api_connection_v1_connection_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


