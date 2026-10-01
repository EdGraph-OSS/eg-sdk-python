# EnrollmentApiEnrollmentRegistrationsV1PathwayMessage

Pathway (the pathway/screen catalog entity) is unrelated to the Registration/Application  rename and is not touched here - only the message name below stays as-is.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**type** | **str** |  | [optional] 
**version** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.enrollment_api_enrollment_registrations_v1_pathway_message import EnrollmentApiEnrollmentRegistrationsV1PathwayMessage

# TODO update the JSON string below
json = "{}"
# create an instance of EnrollmentApiEnrollmentRegistrationsV1PathwayMessage from a JSON string
enrollment_api_enrollment_registrations_v1_pathway_message_instance = EnrollmentApiEnrollmentRegistrationsV1PathwayMessage.from_json(json)
# print the JSON string representation of the object
print(EnrollmentApiEnrollmentRegistrationsV1PathwayMessage.to_json())

# convert the object into a dict
enrollment_api_enrollment_registrations_v1_pathway_message_dict = enrollment_api_enrollment_registrations_v1_pathway_message_instance.to_dict()
# create an instance of EnrollmentApiEnrollmentRegistrationsV1PathwayMessage from a dict
enrollment_api_enrollment_registrations_v1_pathway_message_from_dict = EnrollmentApiEnrollmentRegistrationsV1PathwayMessage.from_dict(enrollment_api_enrollment_registrations_v1_pathway_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


