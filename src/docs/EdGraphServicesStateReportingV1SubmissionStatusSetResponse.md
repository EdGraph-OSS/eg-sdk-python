# EdGraphServicesStateReportingV1SubmissionStatusSetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**submission_id** | **str** |  | [optional] 
**status** | [**EdGraphServicesStateReportingV1SubmissionStatus**](EdGraphServicesStateReportingV1SubmissionStatus.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_submission_status_set_response import EdGraphServicesStateReportingV1SubmissionStatusSetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1SubmissionStatusSetResponse from a JSON string
ed_graph_services_state_reporting_v1_submission_status_set_response_instance = EdGraphServicesStateReportingV1SubmissionStatusSetResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1SubmissionStatusSetResponse.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_submission_status_set_response_dict = ed_graph_services_state_reporting_v1_submission_status_set_response_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1SubmissionStatusSetResponse from a dict
ed_graph_services_state_reporting_v1_submission_status_set_response_from_dict = EdGraphServicesStateReportingV1SubmissionStatusSetResponse.from_dict(ed_graph_services_state_reporting_v1_submission_status_set_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


