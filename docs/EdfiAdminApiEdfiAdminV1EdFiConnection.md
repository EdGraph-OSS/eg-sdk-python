# EdfiAdminApiEdfiAdminV1EdFiConnection


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**connection_name** | **str** |  | [optional] 
**database_engine** | **str** |  | [optional] 
**ed_fi_version** | **str** |  | [optional] 
**ed_fi_extension** | **str** |  | [optional] 
**hosting_provider** | **str** |  | [optional] 
**allowed_tenant_ids** | **List[str]** |  | [optional] [readonly] 
**tiers** | [**List[EdfiAdminApiEdfiAdminV1EdFiConnectionTier]**](EdfiAdminApiEdfiAdminV1EdFiConnectionTier.md) |  | [optional] [readonly] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**connection_type** | **str** |  | [optional] 
**instance_type** | [**EdfiAdminApiEdfiAdminV1InstanceType**](EdfiAdminApiEdfiAdminV1InstanceType.md) |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**metadata_json** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ed_fi_connection import EdfiAdminApiEdfiAdminV1EdFiConnection

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1EdFiConnection from a JSON string
edfi_admin_api_edfi_admin_v1_ed_fi_connection_instance = EdfiAdminApiEdfiAdminV1EdFiConnection.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1EdFiConnection.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_ed_fi_connection_dict = edfi_admin_api_edfi_admin_v1_ed_fi_connection_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1EdFiConnection from a dict
edfi_admin_api_edfi_admin_v1_ed_fi_connection_from_dict = EdfiAdminApiEdfiAdminV1EdFiConnection.from_dict(edfi_admin_api_edfi_admin_v1_ed_fi_connection_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


