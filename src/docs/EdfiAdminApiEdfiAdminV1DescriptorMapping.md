# EdfiAdminApiEdfiAdminV1DescriptorMapping


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**mapped_namespace** | **str** |  | [optional] 
**mapped_value** | **str** |  | [optional] 
**namespace** | **str** |  | [optional] 
**value** | **str** |  | [optional] 
**model_entities** | [**List[EdfiAdminApiEdfiAdminV1DescriptorMappingModelEntity]**](EdfiAdminApiEdfiAdminV1DescriptorMappingModelEntity.md) |  | [optional] [readonly] 
**etag** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_descriptor_mapping import EdfiAdminApiEdfiAdminV1DescriptorMapping

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1DescriptorMapping from a JSON string
edfi_admin_api_edfi_admin_v1_descriptor_mapping_instance = EdfiAdminApiEdfiAdminV1DescriptorMapping.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1DescriptorMapping.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_descriptor_mapping_dict = edfi_admin_api_edfi_admin_v1_descriptor_mapping_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1DescriptorMapping from a dict
edfi_admin_api_edfi_admin_v1_descriptor_mapping_from_dict = EdfiAdminApiEdfiAdminV1DescriptorMapping.from_dict(edfi_admin_api_edfi_admin_v1_descriptor_mapping_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


