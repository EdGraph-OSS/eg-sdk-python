# EdfiAdminApiEdfiAdminV1DescriptorCreatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**descriptor_id** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_descriptor_created_response import EdfiAdminApiEdfiAdminV1DescriptorCreatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1DescriptorCreatedResponse from a JSON string
edfi_admin_api_edfi_admin_v1_descriptor_created_response_instance = EdfiAdminApiEdfiAdminV1DescriptorCreatedResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1DescriptorCreatedResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_descriptor_created_response_dict = edfi_admin_api_edfi_admin_v1_descriptor_created_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1DescriptorCreatedResponse from a dict
edfi_admin_api_edfi_admin_v1_descriptor_created_response_from_dict = EdfiAdminApiEdfiAdminV1DescriptorCreatedResponse.from_dict(edfi_admin_api_edfi_admin_v1_descriptor_created_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


