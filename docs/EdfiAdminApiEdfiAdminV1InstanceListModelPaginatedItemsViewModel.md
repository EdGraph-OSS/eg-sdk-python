# EdfiAdminApiEdfiAdminV1InstanceListModelPaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EdfiAdminApiEdfiAdminV1InstanceListModel]**](EdfiAdminApiEdfiAdminV1InstanceListModel.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_list_model_paginated_items_view_model import EdfiAdminApiEdfiAdminV1InstanceListModelPaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1InstanceListModelPaginatedItemsViewModel from a JSON string
edfi_admin_api_edfi_admin_v1_instance_list_model_paginated_items_view_model_instance = EdfiAdminApiEdfiAdminV1InstanceListModelPaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1InstanceListModelPaginatedItemsViewModel.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_instance_list_model_paginated_items_view_model_dict = edfi_admin_api_edfi_admin_v1_instance_list_model_paginated_items_view_model_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1InstanceListModelPaginatedItemsViewModel from a dict
edfi_admin_api_edfi_admin_v1_instance_list_model_paginated_items_view_model_from_dict = EdfiAdminApiEdfiAdminV1InstanceListModelPaginatedItemsViewModel.from_dict(edfi_admin_api_edfi_admin_v1_instance_list_model_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


