# EdfiAdminApiEdfiAdminV1InstanceDatabase


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**selected_tier_id** | **str** |  | [optional] 
**selected_tier_name** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**jobs** | [**EdfiAdminApiEdfiAdminV1InstanceDatabaseJobs**](EdfiAdminApiEdfiAdminV1InstanceDatabaseJobs.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_database import EdfiAdminApiEdfiAdminV1InstanceDatabase

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1InstanceDatabase from a JSON string
edfi_admin_api_edfi_admin_v1_instance_database_instance = EdfiAdminApiEdfiAdminV1InstanceDatabase.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1InstanceDatabase.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_instance_database_dict = edfi_admin_api_edfi_admin_v1_instance_database_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1InstanceDatabase from a dict
edfi_admin_api_edfi_admin_v1_instance_database_from_dict = EdfiAdminApiEdfiAdminV1InstanceDatabase.from_dict(edfi_admin_api_edfi_admin_v1_instance_database_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


