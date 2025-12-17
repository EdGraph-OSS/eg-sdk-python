# ValidationsApiReportingPeriodsV1SubmissionMetricsDetails


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ed_fi_resource** | **str** |  | [optional] 
**succeeded_count** | **int** |  | [optional] 
**failed_count** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_submission_metrics_details import ValidationsApiReportingPeriodsV1SubmissionMetricsDetails

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1SubmissionMetricsDetails from a JSON string
validations_api_reporting_periods_v1_submission_metrics_details_instance = ValidationsApiReportingPeriodsV1SubmissionMetricsDetails.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1SubmissionMetricsDetails.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_submission_metrics_details_dict = validations_api_reporting_periods_v1_submission_metrics_details_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1SubmissionMetricsDetails from a dict
validations_api_reporting_periods_v1_submission_metrics_details_from_dict = ValidationsApiReportingPeriodsV1SubmissionMetricsDetails.from_dict(validations_api_reporting_periods_v1_submission_metrics_details_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


