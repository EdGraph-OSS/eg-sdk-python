# EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**pathway** | [**EnrollmentApiEnrollmentRegistrationsV1PathwayMessage**](EnrollmentApiEnrollmentRegistrationsV1PathwayMessage.md) |  | [optional] 
**current_screen_code** | **str** |  | [optional] 
**progress** | **str** | Decimal progress (0-100, 2dp) carried as an invariant-culture string,  mirroring the legacy enrollmentresults.proto completedProgress convention. | [optional] 
**language_code** | **str** |  | [optional] 
**contacts** | [**List[EnrollmentApiEnrollmentRegistrationsV1RegistrationContactMessage]**](EnrollmentApiEnrollmentRegistrationsV1RegistrationContactMessage.md) |  | [optional] [readonly] 
**screens** | [**List[EnrollmentApiEnrollmentRegistrationsV1RegistrationScreenMessage]**](EnrollmentApiEnrollmentRegistrationsV1RegistrationScreenMessage.md) |  | [optional] [readonly] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**status** | **str** |  | [optional] 
**next_school_state_short_code** | **str** |  | [optional] 
**next_school_name** | **str** |  | [optional] 
**student** | [**EnrollmentApiEnrollmentRegistrationsV1RegistrationStudentMessage**](EnrollmentApiEnrollmentRegistrationsV1RegistrationStudentMessage.md) |  | [optional] 
**applications** | [**List[EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationMessage]**](EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationMessage.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.enrollment_api_enrollment_registrations_v1_registration_response import EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse from a JSON string
enrollment_api_enrollment_registrations_v1_registration_response_instance = EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse.from_json(json)
# print the JSON string representation of the object
print(EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse.to_json())

# convert the object into a dict
enrollment_api_enrollment_registrations_v1_registration_response_dict = enrollment_api_enrollment_registrations_v1_registration_response_instance.to_dict()
# create an instance of EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse from a dict
enrollment_api_enrollment_registrations_v1_registration_response_from_dict = EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse.from_dict(enrollment_api_enrollment_registrations_v1_registration_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


