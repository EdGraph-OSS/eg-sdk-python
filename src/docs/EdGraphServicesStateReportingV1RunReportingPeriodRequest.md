# EdGraphServicesStateReportingV1RunReportingPeriodRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**rule_ids** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_run_reporting_period_request import EdGraphServicesStateReportingV1RunReportingPeriodRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1RunReportingPeriodRequest from a JSON string
ed_graph_services_state_reporting_v1_run_reporting_period_request_instance = EdGraphServicesStateReportingV1RunReportingPeriodRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1RunReportingPeriodRequest.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_run_reporting_period_request_dict = ed_graph_services_state_reporting_v1_run_reporting_period_request_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1RunReportingPeriodRequest from a dict
ed_graph_services_state_reporting_v1_run_reporting_period_request_from_dict = EdGraphServicesStateReportingV1RunReportingPeriodRequest.from_dict(ed_graph_services_state_reporting_v1_run_reporting_period_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


