# EdGraphServicesStateReportingV1ReportingPeriodPostedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_posted_response import EdGraphServicesStateReportingV1ReportingPeriodPostedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodPostedResponse from a JSON string
ed_graph_services_state_reporting_v1_reporting_period_posted_response_instance = EdGraphServicesStateReportingV1ReportingPeriodPostedResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1ReportingPeriodPostedResponse.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_reporting_period_posted_response_dict = ed_graph_services_state_reporting_v1_reporting_period_posted_response_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodPostedResponse from a dict
ed_graph_services_state_reporting_v1_reporting_period_posted_response_from_dict = EdGraphServicesStateReportingV1ReportingPeriodPostedResponse.from_dict(ed_graph_services_state_reporting_v1_reporting_period_posted_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


