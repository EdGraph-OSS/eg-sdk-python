# ValidationsApiReportingPeriodsV1ValidationSummaryByCategoryId


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reporting_period** | [**ValidationsApiReportingPeriodsV1ReportingPeriodDto**](ValidationsApiReportingPeriodsV1ReportingPeriodDto.md) |  | [optional] 
**category** | [**ValidationsApiContainersV1ContainerDto**](ValidationsApiContainersV1ContainerDto.md) |  | [optional] 
**sub_categories** | [**List[ValidationsApiReportingPeriodsV1ValidationSummarySubCategory]**](ValidationsApiReportingPeriodsV1ValidationSummarySubCategory.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_validation_summary_by_category_id import ValidationsApiReportingPeriodsV1ValidationSummaryByCategoryId

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1ValidationSummaryByCategoryId from a JSON string
validations_api_reporting_periods_v1_validation_summary_by_category_id_instance = ValidationsApiReportingPeriodsV1ValidationSummaryByCategoryId.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1ValidationSummaryByCategoryId.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_validation_summary_by_category_id_dict = validations_api_reporting_periods_v1_validation_summary_by_category_id_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1ValidationSummaryByCategoryId from a dict
validations_api_reporting_periods_v1_validation_summary_by_category_id_from_dict = ValidationsApiReportingPeriodsV1ValidationSummaryByCategoryId.from_dict(validations_api_reporting_periods_v1_validation_summary_by_category_id_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


