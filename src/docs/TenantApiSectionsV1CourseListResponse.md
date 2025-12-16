# TenantApiSectionsV1CourseListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**course_code** | **str** |  | [optional] 
**course_title** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_sections_v1_course_list_response import TenantApiSectionsV1CourseListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiSectionsV1CourseListResponse from a JSON string
tenant_api_sections_v1_course_list_response_instance = TenantApiSectionsV1CourseListResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiSectionsV1CourseListResponse.to_json())

# convert the object into a dict
tenant_api_sections_v1_course_list_response_dict = tenant_api_sections_v1_course_list_response_instance.to_dict()
# create an instance of TenantApiSectionsV1CourseListResponse from a dict
tenant_api_sections_v1_course_list_response_from_dict = TenantApiSectionsV1CourseListResponse.from_dict(tenant_api_sections_v1_course_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


