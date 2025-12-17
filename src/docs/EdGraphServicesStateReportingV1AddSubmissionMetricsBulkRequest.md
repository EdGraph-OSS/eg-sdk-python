# EdGraphServicesStateReportingV1AddSubmissionMetricsBulkRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**submission_id** | **str** |  | [optional] 
**details** | [**List[EdGraphServicesStateReportingV1SubmissionMetricsDetails]**](EdGraphServicesStateReportingV1SubmissionMetricsDetails.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_add_submission_metrics_bulk_request import EdGraphServicesStateReportingV1AddSubmissionMetricsBulkRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1AddSubmissionMetricsBulkRequest from a JSON string
ed_graph_services_state_reporting_v1_add_submission_metrics_bulk_request_instance = EdGraphServicesStateReportingV1AddSubmissionMetricsBulkRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1AddSubmissionMetricsBulkRequest.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_add_submission_metrics_bulk_request_dict = ed_graph_services_state_reporting_v1_add_submission_metrics_bulk_request_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1AddSubmissionMetricsBulkRequest from a dict
ed_graph_services_state_reporting_v1_add_submission_metrics_bulk_request_from_dict = EdGraphServicesStateReportingV1AddSubmissionMetricsBulkRequest.from_dict(ed_graph_services_state_reporting_v1_add_submission_metrics_bulk_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


