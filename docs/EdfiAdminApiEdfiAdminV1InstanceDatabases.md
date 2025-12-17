# EdfiAdminApiEdfiAdminV1InstanceDatabases


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**admin** | [**EdfiAdminApiEdfiAdminV1InstanceDatabase**](EdfiAdminApiEdfiAdminV1InstanceDatabase.md) |  | [optional] 
**security** | [**EdfiAdminApiEdfiAdminV1InstanceDatabase**](EdfiAdminApiEdfiAdminV1InstanceDatabase.md) |  | [optional] 
**ods** | [**List[EdfiAdminApiEdfiAdminV1InstanceOdsDatabase]**](EdfiAdminApiEdfiAdminV1InstanceOdsDatabase.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_databases import EdfiAdminApiEdfiAdminV1InstanceDatabases

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1InstanceDatabases from a JSON string
edfi_admin_api_edfi_admin_v1_instance_databases_instance = EdfiAdminApiEdfiAdminV1InstanceDatabases.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1InstanceDatabases.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_instance_databases_dict = edfi_admin_api_edfi_admin_v1_instance_databases_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1InstanceDatabases from a dict
edfi_admin_api_edfi_admin_v1_instance_databases_from_dict = EdfiAdminApiEdfiAdminV1InstanceDatabases.from_dict(edfi_admin_api_edfi_admin_v1_instance_databases_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


