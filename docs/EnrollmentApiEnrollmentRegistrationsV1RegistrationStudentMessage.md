# EnrollmentApiEnrollmentRegistrationsV1RegistrationStudentMessage

The student a registration is for. studentId is the EnrollmentStudent record id, all zeros until  the registration is linked; the local/state/external ids and names are denormalized from the  student or supplied by the registration flow. No id of its own.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**student_id** | **str** |  | [optional] 
**student_local_code** | **str** |  | [optional] 
**student_state_code** | **str** |  | [optional] 
**student_first_name** | **str** |  | [optional] 
**student_last_name** | **str** |  | [optional] 
**external_data_source_student_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.enrollment_api_enrollment_registrations_v1_registration_student_message import EnrollmentApiEnrollmentRegistrationsV1RegistrationStudentMessage

# TODO update the JSON string below
json = "{}"
# create an instance of EnrollmentApiEnrollmentRegistrationsV1RegistrationStudentMessage from a JSON string
enrollment_api_enrollment_registrations_v1_registration_student_message_instance = EnrollmentApiEnrollmentRegistrationsV1RegistrationStudentMessage.from_json(json)
# print the JSON string representation of the object
print(EnrollmentApiEnrollmentRegistrationsV1RegistrationStudentMessage.to_json())

# convert the object into a dict
enrollment_api_enrollment_registrations_v1_registration_student_message_dict = enrollment_api_enrollment_registrations_v1_registration_student_message_instance.to_dict()
# create an instance of EnrollmentApiEnrollmentRegistrationsV1RegistrationStudentMessage from a dict
enrollment_api_enrollment_registrations_v1_registration_student_message_from_dict = EnrollmentApiEnrollmentRegistrationsV1RegistrationStudentMessage.from_dict(enrollment_api_enrollment_registrations_v1_registration_student_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


