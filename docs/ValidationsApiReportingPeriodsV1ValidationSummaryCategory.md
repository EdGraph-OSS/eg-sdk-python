# ValidationsApiReportingPeriodsV1ValidationSummaryCategory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**category** | [**ValidationsApiContainersV1ContainerDto**](ValidationsApiContainersV1ContainerDto.md) |  | [optional] 
**sub_categories** | [**List[ValidationsApiReportingPeriodsV1ValidationSummarySubCategory]**](ValidationsApiReportingPeriodsV1ValidationSummarySubCategory.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_validation_summary_category import ValidationsApiReportingPeriodsV1ValidationSummaryCategory

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1ValidationSummaryCategory from a JSON string
validations_api_reporting_periods_v1_validation_summary_category_instance = ValidationsApiReportingPeriodsV1ValidationSummaryCategory.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1ValidationSummaryCategory.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_validation_summary_category_dict = validations_api_reporting_periods_v1_validation_summary_category_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1ValidationSummaryCategory from a dict
validations_api_reporting_periods_v1_validation_summary_category_from_dict = ValidationsApiReportingPeriodsV1ValidationSummaryCategory.from_dict(validations_api_reporting_periods_v1_validation_summary_category_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


