# DataSyncApiJobTypeV1JobMetadataField


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
from edgraph_platform_client.models.data_sync_api_job_type_v1_job_metadata_field import DataSyncApiJobTypeV1JobMetadataField

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobTypeV1JobMetadataField from a JSON string
data_sync_api_job_type_v1_job_metadata_field_instance = DataSyncApiJobTypeV1JobMetadataField.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobTypeV1JobMetadataField.to_json())

# convert the object into a dict
data_sync_api_job_type_v1_job_metadata_field_dict = data_sync_api_job_type_v1_job_metadata_field_instance.to_dict()
# create an instance of DataSyncApiJobTypeV1JobMetadataField from a dict
data_sync_api_job_type_v1_job_metadata_field_from_dict = DataSyncApiJobTypeV1JobMetadataField.from_dict(data_sync_api_job_type_v1_job_metadata_field_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


