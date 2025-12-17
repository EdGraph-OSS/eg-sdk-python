# EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponsePaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponse]**](EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_applications_list_response_paginated_items_view_model import EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponsePaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponsePaginatedItemsViewModel from a JSON string
edfi_admin_api_edfi_admin_v1_instance_applications_list_response_paginated_items_view_model_instance = EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponsePaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponsePaginatedItemsViewModel.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_instance_applications_list_response_paginated_items_view_model_dict = edfi_admin_api_edfi_admin_v1_instance_applications_list_response_paginated_items_view_model_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponsePaginatedItemsViewModel from a dict
edfi_admin_api_edfi_admin_v1_instance_applications_list_response_paginated_items_view_model_from_dict = EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponsePaginatedItemsViewModel.from_dict(edfi_admin_api_edfi_admin_v1_instance_applications_list_response_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


