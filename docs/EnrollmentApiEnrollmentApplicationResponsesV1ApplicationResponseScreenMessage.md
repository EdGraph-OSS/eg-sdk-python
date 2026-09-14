# EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseScreenMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**index** | **int** |  | [optional] 
**code** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**updated_by** | **str** |  | [optional] 
**updated_date_time** | **str** |  | [optional] 
**data** | [**GoogleProtobufWellKnownTypesStruct**](GoogleProtobufWellKnownTypesStruct.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.enrollment_api_enrollment_application_responses_v1_application_response_screen_message import EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseScreenMessage

# TODO update the JSON string below
json = "{}"
# create an instance of EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseScreenMessage from a JSON string
enrollment_api_enrollment_application_responses_v1_application_response_screen_message_instance = EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseScreenMessage.from_json(json)
# print the JSON string representation of the object
print(EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseScreenMessage.to_json())

# convert the object into a dict
enrollment_api_enrollment_application_responses_v1_application_response_screen_message_dict = enrollment_api_enrollment_application_responses_v1_application_response_screen_message_instance.to_dict()
# create an instance of EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseScreenMessage from a dict
enrollment_api_enrollment_application_responses_v1_application_response_screen_message_from_dict = EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseScreenMessage.from_dict(enrollment_api_enrollment_application_responses_v1_application_response_screen_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


