# DataSyncApiDslV1JobCreatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_dsl_v1_job_created_response import DataSyncApiDslV1JobCreatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiDslV1JobCreatedResponse from a JSON string
data_sync_api_dsl_v1_job_created_response_instance = DataSyncApiDslV1JobCreatedResponse.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiDslV1JobCreatedResponse.to_json())

# convert the object into a dict
data_sync_api_dsl_v1_job_created_response_dict = data_sync_api_dsl_v1_job_created_response_instance.to_dict()
# create an instance of DataSyncApiDslV1JobCreatedResponse from a dict
data_sync_api_dsl_v1_job_created_response_from_dict = DataSyncApiDslV1JobCreatedResponse.from_dict(data_sync_api_dsl_v1_job_created_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


