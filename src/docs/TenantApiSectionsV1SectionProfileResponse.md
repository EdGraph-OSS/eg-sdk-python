# TenantApiSectionsV1SectionProfileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**section_id** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**school_id** | **int** |  | [optional] 
**school_name** | **str** |  | [optional] 
**session_name** | **str** |  | [optional] 
**term** | **str** |  | [optional] 
**local_course_code** | **str** |  | [optional] 
**local_course_title** | **str** |  | [optional] 
**course_code** | **str** |  | [optional] 
**course_title** | **str** |  | [optional] 
**academic_subjects** | **List[str]** |  | [optional] [readonly] 
**offered_grade_levels** | **List[str]** |  | [optional] [readonly] 
**section_identifier** | **str** |  | [optional] 
**section_name** | **str** |  | [optional] 
**section_type** | **str** |  | [optional] 
**source** | [**TenantApiSectionsV1SectionSource**](TenantApiSectionsV1SectionSource.md) |  | [optional] 
**ed_fi_instance_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**job_execution_id** | **str** |  | [optional] 
**school_year** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_sections_v1_section_profile_response import TenantApiSectionsV1SectionProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiSectionsV1SectionProfileResponse from a JSON string
tenant_api_sections_v1_section_profile_response_instance = TenantApiSectionsV1SectionProfileResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiSectionsV1SectionProfileResponse.to_json())

# convert the object into a dict
tenant_api_sections_v1_section_profile_response_dict = tenant_api_sections_v1_section_profile_response_instance.to_dict()
# create an instance of TenantApiSectionsV1SectionProfileResponse from a dict
tenant_api_sections_v1_section_profile_response_from_dict = TenantApiSectionsV1SectionProfileResponse.from_dict(tenant_api_sections_v1_section_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


