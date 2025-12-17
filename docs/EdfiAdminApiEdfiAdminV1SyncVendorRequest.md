# EdfiAdminApiEdfiAdminV1SyncVendorRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**year** | **int** |  | [optional] 
**vendor_id** | **int** |  | [optional] 
**entries** | [**List[EdfiAdminApiEdfiAdminV1SyncEntry]**](EdfiAdminApiEdfiAdminV1SyncEntry.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_sync_vendor_request import EdfiAdminApiEdfiAdminV1SyncVendorRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1SyncVendorRequest from a JSON string
edfi_admin_api_edfi_admin_v1_sync_vendor_request_instance = EdfiAdminApiEdfiAdminV1SyncVendorRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1SyncVendorRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_sync_vendor_request_dict = edfi_admin_api_edfi_admin_v1_sync_vendor_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1SyncVendorRequest from a dict
edfi_admin_api_edfi_admin_v1_sync_vendor_request_from_dict = EdfiAdminApiEdfiAdminV1SyncVendorRequest.from_dict(edfi_admin_api_edfi_admin_v1_sync_vendor_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


