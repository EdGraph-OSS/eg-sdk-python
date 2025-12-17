# DataSyncApiProviderV1ConnectionType


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**provider_id** | **str** |  | [optional] 
**connection_type_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**documentation_uri** | **str** |  | [optional] 
**connection_metadata_fields** | [**List[DataSyncApiProviderV1ConnectionMetadataField]**](DataSyncApiProviderV1ConnectionMetadataField.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_provider_v1_connection_type import DataSyncApiProviderV1ConnectionType

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiProviderV1ConnectionType from a JSON string
data_sync_api_provider_v1_connection_type_instance = DataSyncApiProviderV1ConnectionType.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiProviderV1ConnectionType.to_json())

# convert the object into a dict
data_sync_api_provider_v1_connection_type_dict = data_sync_api_provider_v1_connection_type_instance.to_dict()
# create an instance of DataSyncApiProviderV1ConnectionType from a dict
data_sync_api_provider_v1_connection_type_from_dict = DataSyncApiProviderV1ConnectionType.from_dict(data_sync_api_provider_v1_connection_type_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


