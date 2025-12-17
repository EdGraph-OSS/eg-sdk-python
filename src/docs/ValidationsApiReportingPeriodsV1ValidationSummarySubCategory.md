# ValidationsApiReportingPeriodsV1ValidationSummarySubCategory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sub_category** | [**ValidationsApiContainersV1ContainerDto**](ValidationsApiContainersV1ContainerDto.md) |  | [optional] 
**rules** | [**List[ValidationsApiRulesV1RuleDto]**](ValidationsApiRulesV1RuleDto.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_validation_summary_sub_category import ValidationsApiReportingPeriodsV1ValidationSummarySubCategory

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1ValidationSummarySubCategory from a JSON string
validations_api_reporting_periods_v1_validation_summary_sub_category_instance = ValidationsApiReportingPeriodsV1ValidationSummarySubCategory.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1ValidationSummarySubCategory.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_validation_summary_sub_category_dict = validations_api_reporting_periods_v1_validation_summary_sub_category_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1ValidationSummarySubCategory from a dict
validations_api_reporting_periods_v1_validation_summary_sub_category_from_dict = ValidationsApiReportingPeriodsV1ValidationSummarySubCategory.from_dict(validations_api_reporting_periods_v1_validation_summary_sub_category_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


