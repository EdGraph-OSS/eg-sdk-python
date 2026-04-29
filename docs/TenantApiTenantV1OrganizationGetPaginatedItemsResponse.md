# TenantApiTenantV1OrganizationGetPaginatedItemsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**data** | [**List[TenantApiTenantV1Organization]**](TenantApiTenantV1Organization.md) |  | [optional] 
**count** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_organization_get_paginated_items_response import TenantApiTenantV1OrganizationGetPaginatedItemsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1OrganizationGetPaginatedItemsResponse from a JSON string
tenant_api_tenant_v1_organization_get_paginated_items_response_instance = TenantApiTenantV1OrganizationGetPaginatedItemsResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1OrganizationGetPaginatedItemsResponse.to_json())

# convert the object into a dict
tenant_api_tenant_v1_organization_get_paginated_items_response_dict = tenant_api_tenant_v1_organization_get_paginated_items_response_instance.to_dict()
# create an instance of TenantApiTenantV1OrganizationGetPaginatedItemsResponse from a dict
tenant_api_tenant_v1_organization_get_paginated_items_response_from_dict = TenantApiTenantV1OrganizationGetPaginatedItemsResponse.from_dict(tenant_api_tenant_v1_organization_get_paginated_items_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


