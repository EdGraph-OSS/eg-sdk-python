# EnrollmentApiEnrollmentStudentsV1StudentResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**student_id** | **str** |  | [optional] 
**allowed_application_profile_ids** | [**List[EnrollmentApiEnrollmentStudentsV1AllowedApplicationProfileIdMessage]**](EnrollmentApiEnrollmentStudentsV1AllowedApplicationProfileIdMessage.md) |  | [optional] [readonly] 
**first_name** | **str** |  | [optional] 
**middle_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**birthdate** | **str** |  | [optional] 
**local_id** | **str** |  | [optional] 
**peims_id** | **str** |  | [optional] 
**last4_ssn** | **str** |  | [optional] 
**next_address** | **str** |  | [optional] 
**next_grade_level** | **str** |  | [optional] 
**next_school_code** | **str** |  | [optional] 
**next_school_name** | **str** |  | [optional] 
**next_school_address** | **str** |  | [optional] 
**eligibility_code** | **str** |  | [optional] 
**eligibility_description** | **str** |  | [optional] 
**contacts** | [**List[EnrollmentApiEnrollmentStudentsV1StudentContactMessage]**](EnrollmentApiEnrollmentStudentsV1StudentContactMessage.md) |  | [optional] [readonly] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.enrollment_api_enrollment_students_v1_student_response import EnrollmentApiEnrollmentStudentsV1StudentResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EnrollmentApiEnrollmentStudentsV1StudentResponse from a JSON string
enrollment_api_enrollment_students_v1_student_response_instance = EnrollmentApiEnrollmentStudentsV1StudentResponse.from_json(json)
# print the JSON string representation of the object
print(EnrollmentApiEnrollmentStudentsV1StudentResponse.to_json())

# convert the object into a dict
enrollment_api_enrollment_students_v1_student_response_dict = enrollment_api_enrollment_students_v1_student_response_instance.to_dict()
# create an instance of EnrollmentApiEnrollmentStudentsV1StudentResponse from a dict
enrollment_api_enrollment_students_v1_student_response_from_dict = EnrollmentApiEnrollmentStudentsV1StudentResponse.from_dict(enrollment_api_enrollment_students_v1_student_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


