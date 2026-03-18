# DataSyncApiDslV1DslProfile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**dag_workflow** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_dsl_v1_dsl_profile import DataSyncApiDslV1DslProfile

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiDslV1DslProfile from a JSON string
data_sync_api_dsl_v1_dsl_profile_instance = DataSyncApiDslV1DslProfile.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiDslV1DslProfile.to_json())

# convert the object into a dict
data_sync_api_dsl_v1_dsl_profile_dict = data_sync_api_dsl_v1_dsl_profile_instance.to_dict()
# create an instance of DataSyncApiDslV1DslProfile from a dict
data_sync_api_dsl_v1_dsl_profile_from_dict = DataSyncApiDslV1DslProfile.from_dict(data_sync_api_dsl_v1_dsl_profile_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


