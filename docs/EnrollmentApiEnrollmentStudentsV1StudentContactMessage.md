# EnrollmentApiEnrollmentStudentsV1StudentContactMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contact_id** | **str** |  | [optional] 
**priority** | **int** |  | [optional] 
**full_name** | **str** |  | [optional] 
**relationship** | **str** |  | [optional] 
**lives_with_student** | **bool** |  | [optional] 
**has_legal_custody** | **bool** |  | [optional] 
**can_pick_up** | **bool** |  | [optional] 
**is_emergency** | **bool** |  | [optional] 
**person_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.enrollment_api_enrollment_students_v1_student_contact_message import EnrollmentApiEnrollmentStudentsV1StudentContactMessage

# TODO update the JSON string below
json = "{}"
# create an instance of EnrollmentApiEnrollmentStudentsV1StudentContactMessage from a JSON string
enrollment_api_enrollment_students_v1_student_contact_message_instance = EnrollmentApiEnrollmentStudentsV1StudentContactMessage.from_json(json)
# print the JSON string representation of the object
print(EnrollmentApiEnrollmentStudentsV1StudentContactMessage.to_json())

# convert the object into a dict
enrollment_api_enrollment_students_v1_student_contact_message_dict = enrollment_api_enrollment_students_v1_student_contact_message_instance.to_dict()
# create an instance of EnrollmentApiEnrollmentStudentsV1StudentContactMessage from a dict
enrollment_api_enrollment_students_v1_student_contact_message_from_dict = EnrollmentApiEnrollmentStudentsV1StudentContactMessage.from_dict(enrollment_api_enrollment_students_v1_student_contact_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


