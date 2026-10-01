# EnrollmentApiEnrollmentRegistrationsV1RegistrationScreenMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**index** | **int** |  | [optional] 
**code** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**data** | [**GoogleProtobufWellKnownTypesStruct**](GoogleProtobufWellKnownTypesStruct.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.enrollment_api_enrollment_registrations_v1_registration_screen_message import EnrollmentApiEnrollmentRegistrationsV1RegistrationScreenMessage

# TODO update the JSON string below
json = "{}"
# create an instance of EnrollmentApiEnrollmentRegistrationsV1RegistrationScreenMessage from a JSON string
enrollment_api_enrollment_registrations_v1_registration_screen_message_instance = EnrollmentApiEnrollmentRegistrationsV1RegistrationScreenMessage.from_json(json)
# print the JSON string representation of the object
print(EnrollmentApiEnrollmentRegistrationsV1RegistrationScreenMessage.to_json())

# convert the object into a dict
enrollment_api_enrollment_registrations_v1_registration_screen_message_dict = enrollment_api_enrollment_registrations_v1_registration_screen_message_instance.to_dict()
# create an instance of EnrollmentApiEnrollmentRegistrationsV1RegistrationScreenMessage from a dict
enrollment_api_enrollment_registrations_v1_registration_screen_message_from_dict = EnrollmentApiEnrollmentRegistrationsV1RegistrationScreenMessage.from_dict(enrollment_api_enrollment_registrations_v1_registration_screen_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


