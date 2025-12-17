# EdGraphServicesStateReportingV1SubmissionMetricsAddedBulkResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**submission_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_submission_metrics_added_bulk_response import EdGraphServicesStateReportingV1SubmissionMetricsAddedBulkResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1SubmissionMetricsAddedBulkResponse from a JSON string
ed_graph_services_state_reporting_v1_submission_metrics_added_bulk_response_instance = EdGraphServicesStateReportingV1SubmissionMetricsAddedBulkResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1SubmissionMetricsAddedBulkResponse.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_submission_metrics_added_bulk_response_dict = ed_graph_services_state_reporting_v1_submission_metrics_added_bulk_response_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1SubmissionMetricsAddedBulkResponse from a dict
ed_graph_services_state_reporting_v1_submission_metrics_added_bulk_response_from_dict = EdGraphServicesStateReportingV1SubmissionMetricsAddedBulkResponse.from_dict(ed_graph_services_state_reporting_v1_submission_metrics_added_bulk_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


