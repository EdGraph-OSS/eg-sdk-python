# EdGraphServicesStateReportingV1ReportingPeriodCurrentStepSetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**number** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_current_step_set_response import EdGraphServicesStateReportingV1ReportingPeriodCurrentStepSetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodCurrentStepSetResponse from a JSON string
ed_graph_services_state_reporting_v1_reporting_period_current_step_set_response_instance = EdGraphServicesStateReportingV1ReportingPeriodCurrentStepSetResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1ReportingPeriodCurrentStepSetResponse.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_reporting_period_current_step_set_response_dict = ed_graph_services_state_reporting_v1_reporting_period_current_step_set_response_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodCurrentStepSetResponse from a dict
ed_graph_services_state_reporting_v1_reporting_period_current_step_set_response_from_dict = EdGraphServicesStateReportingV1ReportingPeriodCurrentStepSetResponse.from_dict(ed_graph_services_state_reporting_v1_reporting_period_current_step_set_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


