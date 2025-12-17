# EdGraphServicesStateReportingV1SubmissionMetricsDetails


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ed_fi_resource** | **str** |  | [optional] 
**succeeded_count** | **int** |  | [optional] 
**failed_count** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_submission_metrics_details import EdGraphServicesStateReportingV1SubmissionMetricsDetails

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1SubmissionMetricsDetails from a JSON string
ed_graph_services_state_reporting_v1_submission_metrics_details_instance = EdGraphServicesStateReportingV1SubmissionMetricsDetails.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1SubmissionMetricsDetails.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_submission_metrics_details_dict = ed_graph_services_state_reporting_v1_submission_metrics_details_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1SubmissionMetricsDetails from a dict
ed_graph_services_state_reporting_v1_submission_metrics_details_from_dict = EdGraphServicesStateReportingV1SubmissionMetricsDetails.from_dict(ed_graph_services_state_reporting_v1_submission_metrics_details_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


