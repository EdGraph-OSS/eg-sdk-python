# EdGraphServicesStateReportingV1ReportingPeriodStep


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**number** | **int** |  | [optional] 
**status** | [**EdGraphServicesStateReportingV1ReportingPeriodStepStatus**](EdGraphServicesStateReportingV1ReportingPeriodStepStatus.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_step import EdGraphServicesStateReportingV1ReportingPeriodStep

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodStep from a JSON string
ed_graph_services_state_reporting_v1_reporting_period_step_instance = EdGraphServicesStateReportingV1ReportingPeriodStep.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1ReportingPeriodStep.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_reporting_period_step_dict = ed_graph_services_state_reporting_v1_reporting_period_step_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodStep from a dict
ed_graph_services_state_reporting_v1_reporting_period_step_from_dict = EdGraphServicesStateReportingV1ReportingPeriodStep.from_dict(ed_graph_services_state_reporting_v1_reporting_period_step_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


