# DataSyncApiConnectionV1ConnectionTestedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | [optional] 
**details** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_connection_v1_connection_tested_response import DataSyncApiConnectionV1ConnectionTestedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiConnectionV1ConnectionTestedResponse from a JSON string
data_sync_api_connection_v1_connection_tested_response_instance = DataSyncApiConnectionV1ConnectionTestedResponse.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiConnectionV1ConnectionTestedResponse.to_json())

# convert the object into a dict
data_sync_api_connection_v1_connection_tested_response_dict = data_sync_api_connection_v1_connection_tested_response_instance.to_dict()
# create an instance of DataSyncApiConnectionV1ConnectionTestedResponse from a dict
data_sync_api_connection_v1_connection_tested_response_from_dict = DataSyncApiConnectionV1ConnectionTestedResponse.from_dict(data_sync_api_connection_v1_connection_tested_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


