# EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponsesSearchResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_size** | **int** |  | [optional] 
**page_index** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseResponse]**](EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponseResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.enrollment_api_enrollment_application_responses_v1_application_responses_search_response import EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponsesSearchResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponsesSearchResponse from a JSON string
enrollment_api_enrollment_application_responses_v1_application_responses_search_response_instance = EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponsesSearchResponse.from_json(json)
# print the JSON string representation of the object
print(EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponsesSearchResponse.to_json())

# convert the object into a dict
enrollment_api_enrollment_application_responses_v1_application_responses_search_response_dict = enrollment_api_enrollment_application_responses_v1_application_responses_search_response_instance.to_dict()
# create an instance of EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponsesSearchResponse from a dict
enrollment_api_enrollment_application_responses_v1_application_responses_search_response_from_dict = EnrollmentApiEnrollmentApplicationResponsesV1ApplicationResponsesSearchResponse.from_dict(enrollment_api_enrollment_application_responses_v1_application_responses_search_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


