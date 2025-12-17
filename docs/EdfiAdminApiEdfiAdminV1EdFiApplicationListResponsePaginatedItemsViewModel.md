# EdfiAdminApiEdfiAdminV1EdFiApplicationListResponsePaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EdfiAdminApiEdfiAdminV1EdFiApplicationListResponse]**](EdfiAdminApiEdfiAdminV1EdFiApplicationListResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ed_fi_application_list_response_paginated_items_view_model import EdfiAdminApiEdfiAdminV1EdFiApplicationListResponsePaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1EdFiApplicationListResponsePaginatedItemsViewModel from a JSON string
edfi_admin_api_edfi_admin_v1_ed_fi_application_list_response_paginated_items_view_model_instance = EdfiAdminApiEdfiAdminV1EdFiApplicationListResponsePaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1EdFiApplicationListResponsePaginatedItemsViewModel.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_ed_fi_application_list_response_paginated_items_view_model_dict = edfi_admin_api_edfi_admin_v1_ed_fi_application_list_response_paginated_items_view_model_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1EdFiApplicationListResponsePaginatedItemsViewModel from a dict
edfi_admin_api_edfi_admin_v1_ed_fi_application_list_response_paginated_items_view_model_from_dict = EdfiAdminApiEdfiAdminV1EdFiApplicationListResponsePaginatedItemsViewModel.from_dict(edfi_admin_api_edfi_admin_v1_ed_fi_application_list_response_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


