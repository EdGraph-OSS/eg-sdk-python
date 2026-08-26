# EnrollmentApiEnrollmentStudentsV1StudentsSearchResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_size** | **int** |  | [optional] 
**page_index** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EnrollmentApiEnrollmentStudentsV1StudentResponse]**](EnrollmentApiEnrollmentStudentsV1StudentResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.enrollment_api_enrollment_students_v1_students_search_response import EnrollmentApiEnrollmentStudentsV1StudentsSearchResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EnrollmentApiEnrollmentStudentsV1StudentsSearchResponse from a JSON string
enrollment_api_enrollment_students_v1_students_search_response_instance = EnrollmentApiEnrollmentStudentsV1StudentsSearchResponse.from_json(json)
# print the JSON string representation of the object
print(EnrollmentApiEnrollmentStudentsV1StudentsSearchResponse.to_json())

# convert the object into a dict
enrollment_api_enrollment_students_v1_students_search_response_dict = enrollment_api_enrollment_students_v1_students_search_response_instance.to_dict()
# create an instance of EnrollmentApiEnrollmentStudentsV1StudentsSearchResponse from a dict
enrollment_api_enrollment_students_v1_students_search_response_from_dict = EnrollmentApiEnrollmentStudentsV1StudentsSearchResponse.from_dict(enrollment_api_enrollment_students_v1_students_search_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


