# EdGraphServicesStateReportingV1AddSubmissionMetricsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**submission_id** | **str** |  | [optional] 
**ed_fi_resource** | **str** |  | [optional] 
**succeeded_count** | **int** |  | [optional] 
**failed_count** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_add_submission_metrics_request import EdGraphServicesStateReportingV1AddSubmissionMetricsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1AddSubmissionMetricsRequest from a JSON string
ed_graph_services_state_reporting_v1_add_submission_metrics_request_instance = EdGraphServicesStateReportingV1AddSubmissionMetricsRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1AddSubmissionMetricsRequest.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_add_submission_metrics_request_dict = ed_graph_services_state_reporting_v1_add_submission_metrics_request_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1AddSubmissionMetricsRequest from a dict
ed_graph_services_state_reporting_v1_add_submission_metrics_request_from_dict = EdGraphServicesStateReportingV1AddSubmissionMetricsRequest.from_dict(ed_graph_services_state_reporting_v1_add_submission_metrics_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


