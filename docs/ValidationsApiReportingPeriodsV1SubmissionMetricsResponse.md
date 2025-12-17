# ValidationsApiReportingPeriodsV1SubmissionMetricsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**submission_id** | **str** |  | [optional] 
**details** | [**List[ValidationsApiReportingPeriodsV1SubmissionMetricsDetails]**](ValidationsApiReportingPeriodsV1SubmissionMetricsDetails.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_submission_metrics_response import ValidationsApiReportingPeriodsV1SubmissionMetricsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1SubmissionMetricsResponse from a JSON string
validations_api_reporting_periods_v1_submission_metrics_response_instance = ValidationsApiReportingPeriodsV1SubmissionMetricsResponse.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1SubmissionMetricsResponse.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_submission_metrics_response_dict = validations_api_reporting_periods_v1_submission_metrics_response_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1SubmissionMetricsResponse from a dict
validations_api_reporting_periods_v1_submission_metrics_response_from_dict = ValidationsApiReportingPeriodsV1SubmissionMetricsResponse.from_dict(validations_api_reporting_periods_v1_submission_metrics_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


