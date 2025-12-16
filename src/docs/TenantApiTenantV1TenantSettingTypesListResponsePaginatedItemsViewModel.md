# TenantApiTenantV1TenantSettingTypesListResponsePaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[TenantApiTenantV1TenantSettingTypesListResponse]**](TenantApiTenantV1TenantSettingTypesListResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_tenant_setting_types_list_response_paginated_items_view_model import TenantApiTenantV1TenantSettingTypesListResponsePaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1TenantSettingTypesListResponsePaginatedItemsViewModel from a JSON string
tenant_api_tenant_v1_tenant_setting_types_list_response_paginated_items_view_model_instance = TenantApiTenantV1TenantSettingTypesListResponsePaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1TenantSettingTypesListResponsePaginatedItemsViewModel.to_json())

# convert the object into a dict
tenant_api_tenant_v1_tenant_setting_types_list_response_paginated_items_view_model_dict = tenant_api_tenant_v1_tenant_setting_types_list_response_paginated_items_view_model_instance.to_dict()
# create an instance of TenantApiTenantV1TenantSettingTypesListResponsePaginatedItemsViewModel from a dict
tenant_api_tenant_v1_tenant_setting_types_list_response_paginated_items_view_model_from_dict = TenantApiTenantV1TenantSettingTypesListResponsePaginatedItemsViewModel.from_dict(tenant_api_tenant_v1_tenant_setting_types_list_response_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


