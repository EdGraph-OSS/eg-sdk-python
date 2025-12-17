# EdfiAdminApiEdfiAdminV1DescriptorMappingsPaginatedItemsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EdfiAdminApiEdfiAdminV1DescriptorMapping]**](EdfiAdminApiEdfiAdminV1DescriptorMapping.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_descriptor_mappings_paginated_items_response import EdfiAdminApiEdfiAdminV1DescriptorMappingsPaginatedItemsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1DescriptorMappingsPaginatedItemsResponse from a JSON string
edfi_admin_api_edfi_admin_v1_descriptor_mappings_paginated_items_response_instance = EdfiAdminApiEdfiAdminV1DescriptorMappingsPaginatedItemsResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1DescriptorMappingsPaginatedItemsResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_descriptor_mappings_paginated_items_response_dict = edfi_admin_api_edfi_admin_v1_descriptor_mappings_paginated_items_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1DescriptorMappingsPaginatedItemsResponse from a dict
edfi_admin_api_edfi_admin_v1_descriptor_mappings_paginated_items_response_from_dict = EdfiAdminApiEdfiAdminV1DescriptorMappingsPaginatedItemsResponse.from_dict(edfi_admin_api_edfi_admin_v1_descriptor_mappings_paginated_items_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


