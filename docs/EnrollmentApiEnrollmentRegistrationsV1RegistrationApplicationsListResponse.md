# EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationsListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationMessage]**](EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationMessage.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.enrollment_api_enrollment_registrations_v1_registration_applications_list_response import EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationsListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationsListResponse from a JSON string
enrollment_api_enrollment_registrations_v1_registration_applications_list_response_instance = EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationsListResponse.from_json(json)
# print the JSON string representation of the object
print(EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationsListResponse.to_json())

# convert the object into a dict
enrollment_api_enrollment_registrations_v1_registration_applications_list_response_dict = enrollment_api_enrollment_registrations_v1_registration_applications_list_response_instance.to_dict()
# create an instance of EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationsListResponse from a dict
enrollment_api_enrollment_registrations_v1_registration_applications_list_response_from_dict = EnrollmentApiEnrollmentRegistrationsV1RegistrationApplicationsListResponse.from_dict(enrollment_api_enrollment_registrations_v1_registration_applications_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


