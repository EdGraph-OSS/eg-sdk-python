# EdfiAdminApiEdfiAdminV1SpecificationsExportedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**type** | [**EdfiAdminApiEdfiAdminV1ExportType**](EdfiAdminApiEdfiAdminV1ExportType.md) |  | [optional] 
**status** | [**EdfiAdminApiEdfiAdminV1ExportStatus**](EdfiAdminApiEdfiAdminV1ExportStatus.md) |  | [optional] 
**details** | **str** |  | [optional] 
**contents** | **List[int]** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_specifications_exported_response import EdfiAdminApiEdfiAdminV1SpecificationsExportedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1SpecificationsExportedResponse from a JSON string
edfi_admin_api_edfi_admin_v1_specifications_exported_response_instance = EdfiAdminApiEdfiAdminV1SpecificationsExportedResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1SpecificationsExportedResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_specifications_exported_response_dict = edfi_admin_api_edfi_admin_v1_specifications_exported_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1SpecificationsExportedResponse from a dict
edfi_admin_api_edfi_admin_v1_specifications_exported_response_from_dict = EdfiAdminApiEdfiAdminV1SpecificationsExportedResponse.from_dict(edfi_admin_api_edfi_admin_v1_specifications_exported_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


