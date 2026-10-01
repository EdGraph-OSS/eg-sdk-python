# EnrollmentApiEnrollmentRegistrationsV1RegistrationsSearchResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_size** | **int** |  | [optional] 
**page_index** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse]**](EnrollmentApiEnrollmentRegistrationsV1RegistrationResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.enrollment_api_enrollment_registrations_v1_registrations_search_response import EnrollmentApiEnrollmentRegistrationsV1RegistrationsSearchResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EnrollmentApiEnrollmentRegistrationsV1RegistrationsSearchResponse from a JSON string
enrollment_api_enrollment_registrations_v1_registrations_search_response_instance = EnrollmentApiEnrollmentRegistrationsV1RegistrationsSearchResponse.from_json(json)
# print the JSON string representation of the object
print(EnrollmentApiEnrollmentRegistrationsV1RegistrationsSearchResponse.to_json())

# convert the object into a dict
enrollment_api_enrollment_registrations_v1_registrations_search_response_dict = enrollment_api_enrollment_registrations_v1_registrations_search_response_instance.to_dict()
# create an instance of EnrollmentApiEnrollmentRegistrationsV1RegistrationsSearchResponse from a dict
enrollment_api_enrollment_registrations_v1_registrations_search_response_from_dict = EnrollmentApiEnrollmentRegistrationsV1RegistrationsSearchResponse.from_dict(enrollment_api_enrollment_registrations_v1_registrations_search_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


