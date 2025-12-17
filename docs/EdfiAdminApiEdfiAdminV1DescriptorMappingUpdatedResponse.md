# EdfiAdminApiEdfiAdminV1DescriptorMappingUpdatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | [optional] 
**previous_mapping_id** | **str** |  | [optional] 
**descriptor_mapping** | [**EdfiAdminApiEdfiAdminV1DescriptorMapping**](EdfiAdminApiEdfiAdminV1DescriptorMapping.md) |  | [optional] 
**details** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_descriptor_mapping_updated_response import EdfiAdminApiEdfiAdminV1DescriptorMappingUpdatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1DescriptorMappingUpdatedResponse from a JSON string
edfi_admin_api_edfi_admin_v1_descriptor_mapping_updated_response_instance = EdfiAdminApiEdfiAdminV1DescriptorMappingUpdatedResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1DescriptorMappingUpdatedResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_descriptor_mapping_updated_response_dict = edfi_admin_api_edfi_admin_v1_descriptor_mapping_updated_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1DescriptorMappingUpdatedResponse from a dict
edfi_admin_api_edfi_admin_v1_descriptor_mapping_updated_response_from_dict = EdfiAdminApiEdfiAdminV1DescriptorMappingUpdatedResponse.from_dict(edfi_admin_api_edfi_admin_v1_descriptor_mapping_updated_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


