# DataSyncApiProviderV1ConnectionMetadataField


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tab** | **str** |  | [optional] 
**code** | **str** |  | [optional] 
**label** | **str** |  | [optional] 
**validation** | **str** |  | [optional] 
**order** | **str** |  | [optional] 
**display** | **bool** |  | [optional] 
**default_value** | **str** |  | [optional] 
**type** | **str** |  | [optional] 
**values** | **str** |  | [optional] 
**api** | **str** |  | [optional] 
**is_secret** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_provider_v1_connection_metadata_field import DataSyncApiProviderV1ConnectionMetadataField

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiProviderV1ConnectionMetadataField from a JSON string
data_sync_api_provider_v1_connection_metadata_field_instance = DataSyncApiProviderV1ConnectionMetadataField.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiProviderV1ConnectionMetadataField.to_json())

# convert the object into a dict
data_sync_api_provider_v1_connection_metadata_field_dict = data_sync_api_provider_v1_connection_metadata_field_instance.to_dict()
# create an instance of DataSyncApiProviderV1ConnectionMetadataField from a dict
data_sync_api_provider_v1_connection_metadata_field_from_dict = DataSyncApiProviderV1ConnectionMetadataField.from_dict(data_sync_api_provider_v1_connection_metadata_field_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


