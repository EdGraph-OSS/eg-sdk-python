# EdGraphServicesStateReportingV1SetReportingPeriodCurrentStepRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**number** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_set_reporting_period_current_step_request import EdGraphServicesStateReportingV1SetReportingPeriodCurrentStepRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1SetReportingPeriodCurrentStepRequest from a JSON string
ed_graph_services_state_reporting_v1_set_reporting_period_current_step_request_instance = EdGraphServicesStateReportingV1SetReportingPeriodCurrentStepRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1SetReportingPeriodCurrentStepRequest.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_set_reporting_period_current_step_request_dict = ed_graph_services_state_reporting_v1_set_reporting_period_current_step_request_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1SetReportingPeriodCurrentStepRequest from a dict
ed_graph_services_state_reporting_v1_set_reporting_period_current_step_request_from_dict = EdGraphServicesStateReportingV1SetReportingPeriodCurrentStepRequest.from_dict(ed_graph_services_state_reporting_v1_set_reporting_period_current_step_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


