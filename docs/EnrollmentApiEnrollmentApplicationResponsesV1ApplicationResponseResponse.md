# EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**application_pathway** | [**EnrollmentApiEnrollmentApplicationResponsesV1ApplicationPathwayMessage**](EnrollmentApiEnrollmentApplicationResponsesV1ApplicationPathwayMessage.md) |  | [optional] 
**current_screen_code** | **str** |  | [optional] 
**progress** | **str** | Decimal progress (0-100, 2dp) carried as an invariant-culture string,  mirroring the legacy enrollmentresults.proto completedProgress convention. | [optional] 
**student_id** | **str** |  | [optional] 
**language_code** | **str** |  | [optional] 
**contacts** | [**List[EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseContactMessage]**](EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseContactMessage.md) |  | [optional] [readonly] 
**screens** | [**List[EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseScreenMessage]**](EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseScreenMessage.md) |  | [optional] [readonly] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**status** | **str** |  | [optional] 
**student_first_name** | **str** |  | [optional] 
**student_last_name** | **str** |  | [optional] 
**student_local_id** | **str** |  | [optional] 
**next_school_code** | **str** |  | [optional] 
**next_school_name** | **str** |  | [optional] 

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


