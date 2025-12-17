# EdfiAdminApiEdfiAdminV1SyncApplicationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**year** | **int** |  | [optional] 
**application_id** | **int** |  | [optional] 
**entries** | [**List[EdfiAdminApiEdfiAdminV1SyncEntry]**](EdfiAdminApiEdfiAdminV1SyncEntry.md) |  | [optional] [readonly] 
**assign_to_existing_leas** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_sync_application_request import EdfiAdminApiEdfiAdminV1SyncApplicationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1SyncApplicationRequest from a JSON string
edfi_admin_api_edfi_admin_v1_sync_application_request_instance = EdfiAdminApiEdfiAdminV1SyncApplicationRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1SyncApplicationRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_sync_application_request_dict = edfi_admin_api_edfi_admin_v1_sync_application_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1SyncApplicationRequest from a dict
edfi_admin_api_edfi_admin_v1_sync_application_request_from_dict = EdfiAdminApiEdfiAdminV1SyncApplicationRequest.from_dict(edfi_admin_api_edfi_admin_v1_sync_application_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


