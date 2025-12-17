# ValidationsApiReportingPeriodsV1AddSubmissionMetricsBulkRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**submission_id** | **str** |  | [optional] 
**details** | [**List[ValidationsApiReportingPeriodsV1SubmissionMetricsDetails]**](ValidationsApiReportingPeriodsV1SubmissionMetricsDetails.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_add_submission_metrics_bulk_request import ValidationsApiReportingPeriodsV1AddSubmissionMetricsBulkRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1AddSubmissionMetricsBulkRequest from a JSON string
validations_api_reporting_periods_v1_add_submission_metrics_bulk_request_instance = ValidationsApiReportingPeriodsV1AddSubmissionMetricsBulkRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1AddSubmissionMetricsBulkRequest.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_add_submission_metrics_bulk_request_dict = validations_api_reporting_periods_v1_add_submission_metrics_bulk_request_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1AddSubmissionMetricsBulkRequest from a dict
validations_api_reporting_periods_v1_add_submission_metrics_bulk_request_from_dict = ValidationsApiReportingPeriodsV1AddSubmissionMetricsBulkRequest.from_dict(validations_api_reporting_periods_v1_add_submission_metrics_bulk_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


