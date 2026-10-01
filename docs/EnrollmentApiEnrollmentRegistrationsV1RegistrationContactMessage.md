# EnrollmentApiEnrollmentRegistrationsV1RegistrationContactMessage

One contact on a registration. id is the entry's own identity (minted once, never overwritten);  contactId is the EnrollmentContact record id the entry resolved to (the key every join goes  through; unset until resolved); externalDataSourceContactId is the SIS-side code, when known.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**contact_id** | **str** |  | [optional] 
**contact_name** | **str** |  | [optional] 
**contact_phone** | **str** |  | [optional] 
**contact_email** | **str** |  | [optional] 
**external_data_source_contact_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.enrollment_api_enrollment_registrations_v1_registration_contact_message import EnrollmentApiEnrollmentRegistrationsV1RegistrationContactMessage

# TODO update the JSON string below
json = "{}"
# create an instance of EnrollmentApiEnrollmentRegistrationsV1RegistrationContactMessage from a JSON string
enrollment_api_enrollment_registrations_v1_registration_contact_message_instance = EnrollmentApiEnrollmentRegistrationsV1RegistrationContactMessage.from_json(json)
# print the JSON string representation of the object
print(EnrollmentApiEnrollmentRegistrationsV1RegistrationContactMessage.to_json())

# convert the object into a dict
enrollment_api_enrollment_registrations_v1_registration_contact_message_dict = enrollment_api_enrollment_registrations_v1_registration_contact_message_instance.to_dict()
# create an instance of EnrollmentApiEnrollmentRegistrationsV1RegistrationContactMessage from a dict
enrollment_api_enrollment_registrations_v1_registration_contact_message_from_dict = EnrollmentApiEnrollmentRegistrationsV1RegistrationContactMessage.from_dict(enrollment_api_enrollment_registrations_v1_registration_contact_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


