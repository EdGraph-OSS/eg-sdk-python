# TenantApiSectionsV1PaginatedAcademicSubjectsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[TenantApiSectionsV1AcademicSubjectListResponse]**](TenantApiSectionsV1AcademicSubjectListResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.tenant_api_sections_v1_paginated_academic_subjects_response import TenantApiSectionsV1PaginatedAcademicSubjectsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiSectionsV1PaginatedAcademicSubjectsResponse from a JSON string
tenant_api_sections_v1_paginated_academic_subjects_response_instance = TenantApiSectionsV1PaginatedAcademicSubjectsResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiSectionsV1PaginatedAcademicSubjectsResponse.to_json())

# convert the object into a dict
tenant_api_sections_v1_paginated_academic_subjects_response_dict = tenant_api_sections_v1_paginated_academic_subjects_response_instance.to_dict()
# create an instance of TenantApiSectionsV1PaginatedAcademicSubjectsResponse from a dict
tenant_api_sections_v1_paginated_academic_subjects_response_from_dict = TenantApiSectionsV1PaginatedAcademicSubjectsResponse.from_dict(tenant_api_sections_v1_paginated_academic_subjects_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


