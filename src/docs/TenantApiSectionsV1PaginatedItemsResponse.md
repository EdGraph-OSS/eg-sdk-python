# TenantApiSectionsV1PaginatedItemsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[TenantApiSectionsV1SectionListResponse]**](TenantApiSectionsV1SectionListResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.tenant_api_sections_v1_paginated_items_response import TenantApiSectionsV1PaginatedItemsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiSectionsV1PaginatedItemsResponse from a JSON string
tenant_api_sections_v1_paginated_items_response_instance = TenantApiSectionsV1PaginatedItemsResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiSectionsV1PaginatedItemsResponse.to_json())

# convert the object into a dict
tenant_api_sections_v1_paginated_items_response_dict = tenant_api_sections_v1_paginated_items_response_instance.to_dict()
# create an instance of TenantApiSectionsV1PaginatedItemsResponse from a dict
tenant_api_sections_v1_paginated_items_response_from_dict = TenantApiSectionsV1PaginatedItemsResponse.from_dict(tenant_api_sections_v1_paginated_items_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


