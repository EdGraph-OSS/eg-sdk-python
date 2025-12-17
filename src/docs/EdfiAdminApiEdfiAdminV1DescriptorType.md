# EdfiAdminApiEdfiAdminV1DescriptorType


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**descriptor_id** | **int** |  | [optional] 
**namespace** | **str** |  | [optional] 
**code_value** | **str** |  | [optional] 
**short_description** | **str** |  | [optional] 
**description** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_descriptor_type import EdfiAdminApiEdfiAdminV1DescriptorType

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1DescriptorType from a JSON string
edfi_admin_api_edfi_admin_v1_descriptor_type_instance = EdfiAdminApiEdfiAdminV1DescriptorType.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1DescriptorType.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_descriptor_type_dict = edfi_admin_api_edfi_admin_v1_descriptor_type_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1DescriptorType from a dict
edfi_admin_api_edfi_admin_v1_descriptor_type_from_dict = EdfiAdminApiEdfiAdminV1DescriptorType.from_dict(edfi_admin_api_edfi_admin_v1_descriptor_type_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


