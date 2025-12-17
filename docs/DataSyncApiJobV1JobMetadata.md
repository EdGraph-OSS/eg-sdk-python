# DataSyncApiJobV1JobMetadata


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | [optional] 
**value** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_v1_job_metadata import DataSyncApiJobV1JobMetadata

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobV1JobMetadata from a JSON string
data_sync_api_job_v1_job_metadata_instance = DataSyncApiJobV1JobMetadata.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobV1JobMetadata.to_json())

# convert the object into a dict
data_sync_api_job_v1_job_metadata_dict = data_sync_api_job_v1_job_metadata_instance.to_dict()
# create an instance of DataSyncApiJobV1JobMetadata from a dict
data_sync_api_job_v1_job_metadata_from_dict = DataSyncApiJobV1JobMetadata.from_dict(data_sync_api_job_v1_job_metadata_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


