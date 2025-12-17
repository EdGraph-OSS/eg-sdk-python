# EdfiAdminApiEdfiAdminV1UpdateDescriptorMappingRequest


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
**instance_id** | **str** |  | [optional] 
**year** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_descriptor_mapping_request import EdfiAdminApiEdfiAdminV1UpdateDescriptorMappingRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1UpdateDescriptorMappingRequest from a JSON string
edfi_admin_api_edfi_admin_v1_update_descriptor_mapping_request_instance = EdfiAdminApiEdfiAdminV1UpdateDescriptorMappingRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1UpdateDescriptorMappingRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_update_descriptor_mapping_request_dict = edfi_admin_api_edfi_admin_v1_update_descriptor_mapping_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1UpdateDescriptorMappingRequest from a dict
edfi_admin_api_edfi_admin_v1_update_descriptor_mapping_request_from_dict = EdfiAdminApiEdfiAdminV1UpdateDescriptorMappingRequest.from_dict(edfi_admin_api_edfi_admin_v1_update_descriptor_mapping_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


