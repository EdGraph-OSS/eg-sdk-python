# EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseContactMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**source_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**phone** | **str** |  | [optional] 
**email** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.enrollment_api_enrollment_application_responses_v1_application_response_contact_message import EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseContactMessage

# TODO update the JSON string below
json = "{}"
# create an instance of EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseContactMessage from a JSON string
enrollment_api_enrollment_application_responses_v1_application_response_contact_message_instance = EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseContactMessage.from_json(json)
# print the JSON string representation of the object
print(EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseContactMessage.to_json())

# convert the object into a dict
enrollment_api_enrollment_application_responses_v1_application_response_contact_message_dict = enrollment_api_enrollment_application_responses_v1_application_response_contact_message_instance.to_dict()
# create an instance of EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseContactMessage from a dict
enrollment_api_enrollment_application_responses_v1_application_response_contact_message_from_dict = EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseContactMessage.from_dict(enrollment_api_enrollment_application_responses_v1_application_response_contact_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


