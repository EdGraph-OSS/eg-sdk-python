# EdGraphServicesStateReportingV1ReportingPeriodValidationSummary


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reporting_period** | [**EdGraphServicesStateReportingV1ReportingPeriodListResponse**](EdGraphServicesStateReportingV1ReportingPeriodListResponse.md) |  | [optional] 
**categories** | [**List[EdGraphServicesStateReportingV1ValidationSummaryCategory]**](EdGraphServicesStateReportingV1ValidationSummaryCategory.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_validation_summary import EdGraphServicesStateReportingV1ReportingPeriodValidationSummary

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodValidationSummary from a JSON string
ed_graph_services_state_reporting_v1_reporting_period_validation_summary_instance = EdGraphServicesStateReportingV1ReportingPeriodValidationSummary.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1ReportingPeriodValidationSummary.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_reporting_period_validation_summary_dict = ed_graph_services_state_reporting_v1_reporting_period_validation_summary_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodValidationSummary from a dict
ed_graph_services_state_reporting_v1_reporting_period_validation_summary_from_dict = EdGraphServicesStateReportingV1ReportingPeriodValidationSummary.from_dict(ed_graph_services_state_reporting_v1_reporting_period_validation_summary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


