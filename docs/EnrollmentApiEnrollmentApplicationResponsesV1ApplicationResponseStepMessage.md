# EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseStepMessage


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
from edgraph_platform_client.models.enrollment_api_enrollment_application_responses_v1_application_response_step_message import EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseStepMessage

# TODO update the JSON string below
json = "{}"
# create an instance of EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseStepMessage from a JSON string
enrollment_api_enrollment_application_responses_v1_application_response_step_message_instance = EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseStepMessage.from_json(json)
# print the JSON string representation of the object
print(EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseStepMessage.to_json())

# convert the object into a dict
enrollment_api_enrollment_application_responses_v1_application_response_step_message_dict = enrollment_api_enrollment_application_responses_v1_application_response_step_message_instance.to_dict()
# create an instance of EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseStepMessage from a dict
enrollment_api_enrollment_application_responses_v1_application_response_step_message_from_dict = EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseStepMessage.from_dict(enrollment_api_enrollment_application_responses_v1_application_response_step_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


