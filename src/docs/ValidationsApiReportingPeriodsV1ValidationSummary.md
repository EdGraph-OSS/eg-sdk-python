# ValidationsApiReportingPeriodsV1ValidationSummary


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reporting_period** | [**ValidationsApiReportingPeriodsV1ReportingPeriodDto**](ValidationsApiReportingPeriodsV1ReportingPeriodDto.md) |  | [optional] 
**categories** | [**List[ValidationsApiReportingPeriodsV1ValidationSummaryCategory]**](ValidationsApiReportingPeriodsV1ValidationSummaryCategory.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_validation_summary import ValidationsApiReportingPeriodsV1ValidationSummary

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1ValidationSummary from a JSON string
validations_api_reporting_periods_v1_validation_summary_instance = ValidationsApiReportingPeriodsV1ValidationSummary.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1ValidationSummary.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_validation_summary_dict = validations_api_reporting_periods_v1_validation_summary_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1ValidationSummary from a dict
validations_api_reporting_periods_v1_validation_summary_from_dict = ValidationsApiReportingPeriodsV1ValidationSummary.from_dict(validations_api_reporting_periods_v1_validation_summary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


