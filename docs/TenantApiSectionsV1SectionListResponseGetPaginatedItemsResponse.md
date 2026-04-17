# TenantApiSectionsV1SectionListResponseGetPaginatedItemsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**data** | [**List[TenantApiSectionsV1SectionListResponse]**](TenantApiSectionsV1SectionListResponse.md) |  | [optional] 
**count** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_sections_v1_section_list_response_get_paginated_items_response import TenantApiSectionsV1SectionListResponseGetPaginatedItemsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiSectionsV1SectionListResponseGetPaginatedItemsResponse from a JSON string
tenant_api_sections_v1_section_list_response_get_paginated_items_response_instance = TenantApiSectionsV1SectionListResponseGetPaginatedItemsResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiSectionsV1SectionListResponseGetPaginatedItemsResponse.to_json())

# convert the object into a dict
tenant_api_sections_v1_section_list_response_get_paginated_items_response_dict = tenant_api_sections_v1_section_list_response_get_paginated_items_response_instance.to_dict()
# create an instance of TenantApiSectionsV1SectionListResponseGetPaginatedItemsResponse from a dict
tenant_api_sections_v1_section_list_response_get_paginated_items_response_from_dict = TenantApiSectionsV1SectionListResponseGetPaginatedItemsResponse.from_dict(tenant_api_sections_v1_section_list_response_get_paginated_items_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


