# TenantApiSectionsV1PaginatedCoursesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[TenantApiSectionsV1CourseListResponse]**](TenantApiSectionsV1CourseListResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.tenant_api_sections_v1_paginated_courses_response import TenantApiSectionsV1PaginatedCoursesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiSectionsV1PaginatedCoursesResponse from a JSON string
tenant_api_sections_v1_paginated_courses_response_instance = TenantApiSectionsV1PaginatedCoursesResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiSectionsV1PaginatedCoursesResponse.to_json())

# convert the object into a dict
tenant_api_sections_v1_paginated_courses_response_dict = tenant_api_sections_v1_paginated_courses_response_instance.to_dict()
# create an instance of TenantApiSectionsV1PaginatedCoursesResponse from a dict
tenant_api_sections_v1_paginated_courses_response_from_dict = TenantApiSectionsV1PaginatedCoursesResponse.from_dict(tenant_api_sections_v1_paginated_courses_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


