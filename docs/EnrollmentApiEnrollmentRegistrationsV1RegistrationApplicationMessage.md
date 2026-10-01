# EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationMessage

One Program-seat choice on a Registration - zero-to-many, independently approvable. See  ApproveRegistrationApplication / GetRegistrationApplications.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**application_id** | **str** |  | [optional] 
**application_status** | **str** |  | [optional] 
**program_id** | **str** | enrollment-svc-programs._id - one school&#39;s offering of a program. | [optional] 
**rank** | **int** | The family&#39;s preference order within the round. 1-based and contiguous across the  registration - the matcher&#39;s contract. Assigned server-side, never supplied by a caller. | [optional] 
**priority** | **int** | The priority tier - sibling, staff, feeder, PreK. Unset until the priority engine stamps it. | [optional] 
**application_round_id** | **str** | Foreign key into the application round this entry was submitted to. | [optional] 

## Example

```python
from edgraph_platform_client.models.enrollment_api_enrollment_registrations_v1_registration_application_message import EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationMessage

# TODO update the JSON string below
json = "{}"
# create an instance of EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationMessage from a JSON string
enrollment_api_enrollment_registrations_v1_registration_application_message_instance = EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationMessage.from_json(json)
# print the JSON string representation of the object
print(EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationMessage.to_json())

# convert the object into a dict
enrollment_api_enrollment_registrations_v1_registration_application_message_dict = enrollment_api_enrollment_registrations_v1_registration_application_message_instance.to_dict()
# create an instance of EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationMessage from a dict
enrollment_api_enrollment_registrations_v1_registration_application_message_from_dict = EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationMessage.from_dict(enrollment_api_enrollment_registrations_v1_registration_application_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


