# DataSyncApiJobTypeV1JobTypeProfileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**job_type_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**job_points** | **int** |  | [optional] 
**has_child_jobs** | **bool** |  | [optional] 
**child_job_field** | **str** |  | [optional] 
**source_connection_type_id** | **str** |  | [optional] 
**destination_connection_type_id** | **str** |  | [optional] 
**source_connection_required** | **bool** |  | [optional] 
**destination_connection_required** | **bool** |  | [optional] 
**job_metadata_fields** | [**List[DataSyncApiJobTypeV1JobMetadataField]**](DataSyncApiJobTypeV1JobMetadataField.md) |  | [optional] [readonly] 
**profiles** | [**List[DataSyncApiJobTypeV1Profile]**](DataSyncApiJobTypeV1Profile.md) |  | [optional] [readonly] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_type_v1_job_type_profile_response import DataSyncApiJobTypeV1JobTypeProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobTypeV1JobTypeProfileResponse from a JSON string
data_sync_api_job_type_v1_job_type_profile_response_instance = DataSyncApiJobTypeV1JobTypeProfileResponse.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobTypeV1JobTypeProfileResponse.to_json())

# convert the object into a dict
data_sync_api_job_type_v1_job_type_profile_response_dict = data_sync_api_job_type_v1_job_type_profile_response_instance.to_dict()
# create an instance of DataSyncApiJobTypeV1JobTypeProfileResponse from a dict
data_sync_api_job_type_v1_job_type_profile_response_from_dict = DataSyncApiJobTypeV1JobTypeProfileResponse.from_dict(data_sync_api_job_type_v1_job_type_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


