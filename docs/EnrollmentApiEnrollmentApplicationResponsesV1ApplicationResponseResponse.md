# EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**application_profile** | [**EnrollmentApiEnrollmentApplicationResponsesV1ApplicationProfileMessage**](EnrollmentApiEnrollmentApplicationResponsesV1ApplicationProfileMessage.md) |  | [optional] 
**current_step_code** | **str** |  | [optional] 
**completed_progress** | **float** |  | [optional] 
**student_id** | **str** |  | [optional] 
**language_code** | **str** |  | [optional] 
**contacts** | [**List[EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseContactMessage]**](EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseContactMessage.md) |  | [optional] [readonly] 
**steps** | [**List[EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseStepMessage]**](EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseStepMessage.md) |  | [optional] [readonly] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.enrollment_api_enrollment_application_responses_v1_application_response_response import EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseResponse from a JSON string
enrollment_api_enrollment_application_responses_v1_application_response_response_instance = EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseResponse.from_json(json)
# print the JSON string representation of the object
print(EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseResponse.to_json())

# convert the object into a dict
enrollment_api_enrollment_application_responses_v1_application_response_response_dict = enrollment_api_enrollment_application_responses_v1_application_response_response_instance.to_dict()
# create an instance of EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseResponse from a dict
enrollment_api_enrollment_application_responses_v1_application_response_response_from_dict = EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseResponse.from_dict(enrollment_api_enrollment_application_responses_v1_application_response_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


