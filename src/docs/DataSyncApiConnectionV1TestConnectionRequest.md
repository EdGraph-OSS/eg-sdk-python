# DataSyncApiConnectionV1TestConnectionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**connection_id** | **str** |  | [optional] 
**provider_id** | **str** |  | [optional] 
**connection_type_id** | **str** |  | [optional] 
**connection_metadata** | [**List[DataSyncApiConnectionV1ConnectionMetadata]**](DataSyncApiConnectionV1ConnectionMetadata.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_connection_v1_test_connection_request import DataSyncApiConnectionV1TestConnectionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiConnectionV1TestConnectionRequest from a JSON string
data_sync_api_connection_v1_test_connection_request_instance = DataSyncApiConnectionV1TestConnectionRequest.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiConnectionV1TestConnectionRequest.to_json())

# convert the object into a dict
data_sync_api_connection_v1_test_connection_request_dict = data_sync_api_connection_v1_test_connection_request_instance.to_dict()
# create an instance of DataSyncApiConnectionV1TestConnectionRequest from a dict
data_sync_api_connection_v1_test_connection_request_from_dict = DataSyncApiConnectionV1TestConnectionRequest.from_dict(data_sync_api_connection_v1_test_connection_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


