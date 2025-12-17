# DataSyncApiConnectionV1ConnectionMetadata


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | [optional] 
**value** | **str** |  | [optional] 
**is_secret** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_connection_v1_connection_metadata import DataSyncApiConnectionV1ConnectionMetadata

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiConnectionV1ConnectionMetadata from a JSON string
data_sync_api_connection_v1_connection_metadata_instance = DataSyncApiConnectionV1ConnectionMetadata.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiConnectionV1ConnectionMetadata.to_json())

# convert the object into a dict
data_sync_api_connection_v1_connection_metadata_dict = data_sync_api_connection_v1_connection_metadata_instance.to_dict()
# create an instance of DataSyncApiConnectionV1ConnectionMetadata from a dict
data_sync_api_connection_v1_connection_metadata_from_dict = DataSyncApiConnectionV1ConnectionMetadata.from_dict(data_sync_api_connection_v1_connection_metadata_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


