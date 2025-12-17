# EdfiAdminApiEdfiAdminV1CreateDescriptorMappingRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**mapped_namespace** | **str** |  | [optional] 
**mapped_value** | **str** |  | [optional] 
**namespace** | **str** |  | [optional] 
**value** | **str** |  | [optional] 
**model_entities** | [**List[EdfiAdminApiEdfiAdminV1DescriptorMappingModelEntity]**](EdfiAdminApiEdfiAdminV1DescriptorMappingModelEntity.md) |  | [optional] [readonly] 
**etag** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**year** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_descriptor_mapping_request import EdfiAdminApiEdfiAdminV1CreateDescriptorMappingRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1CreateDescriptorMappingRequest from a JSON string
edfi_admin_api_edfi_admin_v1_create_descriptor_mapping_request_instance = EdfiAdminApiEdfiAdminV1CreateDescriptorMappingRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1CreateDescriptorMappingRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_create_descriptor_mapping_request_dict = edfi_admin_api_edfi_admin_v1_create_descriptor_mapping_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1CreateDescriptorMappingRequest from a dict
edfi_admin_api_edfi_admin_v1_create_descriptor_mapping_request_from_dict = EdfiAdminApiEdfiAdminV1CreateDescriptorMappingRequest.from_dict(edfi_admin_api_edfi_admin_v1_create_descriptor_mapping_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


