# EdfiAdminApiEdfiAdminV1ExportSpecificationsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**type** | [**EdfiAdminApiEdfiAdminV1ExportType**](EdfiAdminApiEdfiAdminV1ExportType.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_export_specifications_request import EdfiAdminApiEdfiAdminV1ExportSpecificationsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1ExportSpecificationsRequest from a JSON string
edfi_admin_api_edfi_admin_v1_export_specifications_request_instance = EdfiAdminApiEdfiAdminV1ExportSpecificationsRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1ExportSpecificationsRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_export_specifications_request_dict = edfi_admin_api_edfi_admin_v1_export_specifications_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1ExportSpecificationsRequest from a dict
edfi_admin_api_edfi_admin_v1_export_specifications_request_from_dict = EdfiAdminApiEdfiAdminV1ExportSpecificationsRequest.from_dict(edfi_admin_api_edfi_admin_v1_export_specifications_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


