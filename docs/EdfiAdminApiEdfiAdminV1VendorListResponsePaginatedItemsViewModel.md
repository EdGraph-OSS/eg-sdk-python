# EdfiAdminApiEdfiAdminV1VendorListResponsePaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EdfiAdminApiEdfiAdminV1VendorListResponse]**](EdfiAdminApiEdfiAdminV1VendorListResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_vendor_list_response_paginated_items_view_model import EdfiAdminApiEdfiAdminV1VendorListResponsePaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1VendorListResponsePaginatedItemsViewModel from a JSON string
edfi_admin_api_edfi_admin_v1_vendor_list_response_paginated_items_view_model_instance = EdfiAdminApiEdfiAdminV1VendorListResponsePaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1VendorListResponsePaginatedItemsViewModel.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_vendor_list_response_paginated_items_view_model_dict = edfi_admin_api_edfi_admin_v1_vendor_list_response_paginated_items_view_model_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1VendorListResponsePaginatedItemsViewModel from a dict
edfi_admin_api_edfi_admin_v1_vendor_list_response_paginated_items_view_model_from_dict = EdfiAdminApiEdfiAdminV1VendorListResponsePaginatedItemsViewModel.from_dict(edfi_admin_api_edfi_admin_v1_vendor_list_response_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


