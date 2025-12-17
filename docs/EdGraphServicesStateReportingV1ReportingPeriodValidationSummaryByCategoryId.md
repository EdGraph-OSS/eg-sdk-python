# EdGraphServicesStateReportingV1ReportingPeriodValidationSummaryByCategoryId


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reporting_period** | [**EdGraphServicesStateReportingV1ReportingPeriodListResponse**](EdGraphServicesStateReportingV1ReportingPeriodListResponse.md) |  | [optional] 
**category** | [**EdGraphServicesStateReportingV1Category**](EdGraphServicesStateReportingV1Category.md) |  | [optional] 
**sub_categories** | [**List[EdGraphServicesStateReportingV1ValidationSummarySubCategory]**](EdGraphServicesStateReportingV1ValidationSummarySubCategory.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_validation_summary_by_category_id import EdGraphServicesStateReportingV1ReportingPeriodValidationSummaryByCategoryId

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodValidationSummaryByCategoryId from a JSON string
ed_graph_services_state_reporting_v1_reporting_period_validation_summary_by_category_id_instance = EdGraphServicesStateReportingV1ReportingPeriodValidationSummaryByCategoryId.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1ReportingPeriodValidationSummaryByCategoryId.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_reporting_period_validation_summary_by_category_id_dict = ed_graph_services_state_reporting_v1_reporting_period_validation_summary_by_category_id_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodValidationSummaryByCategoryId from a dict
ed_graph_services_state_reporting_v1_reporting_period_validation_summary_by_category_id_from_dict = EdGraphServicesStateReportingV1ReportingPeriodValidationSummaryByCategoryId.from_dict(ed_graph_services_state_reporting_v1_reporting_period_validation_summary_by_category_id_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


