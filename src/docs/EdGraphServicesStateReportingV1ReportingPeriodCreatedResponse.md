# EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_created_response import EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse from a JSON string
ed_graph_services_state_reporting_v1_reporting_period_created_response_instance = EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_reporting_period_created_response_dict = ed_graph_services_state_reporting_v1_reporting_period_created_response_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse from a dict
ed_graph_services_state_reporting_v1_reporting_period_created_response_from_dict = EdGraphServicesStateReportingV1ReportingPeriodCreatedResponse.from_dict(ed_graph_services_state_reporting_v1_reporting_period_created_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


