# EdGraphServicesStateReportingV1SubmissionCancelledResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**submission_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_submission_cancelled_response import EdGraphServicesStateReportingV1SubmissionCancelledResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1SubmissionCancelledResponse from a JSON string
ed_graph_services_state_reporting_v1_submission_cancelled_response_instance = EdGraphServicesStateReportingV1SubmissionCancelledResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1SubmissionCancelledResponse.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_submission_cancelled_response_dict = ed_graph_services_state_reporting_v1_submission_cancelled_response_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1SubmissionCancelledResponse from a dict
ed_graph_services_state_reporting_v1_submission_cancelled_response_from_dict = EdGraphServicesStateReportingV1SubmissionCancelledResponse.from_dict(ed_graph_services_state_reporting_v1_submission_cancelled_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


