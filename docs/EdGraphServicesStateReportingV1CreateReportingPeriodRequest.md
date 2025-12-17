# EdGraphServicesStateReportingV1CreateReportingPeriodRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**tag_id** | **str** |  | [optional] 
**rule_ids** | **List[str]** |  | [optional] [readonly] 
**code** | **str** |  | [optional] 
**display_name** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_create_reporting_period_request import EdGraphServicesStateReportingV1CreateReportingPeriodRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1CreateReportingPeriodRequest from a JSON string
ed_graph_services_state_reporting_v1_create_reporting_period_request_instance = EdGraphServicesStateReportingV1CreateReportingPeriodRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1CreateReportingPeriodRequest.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_create_reporting_period_request_dict = ed_graph_services_state_reporting_v1_create_reporting_period_request_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1CreateReportingPeriodRequest from a dict
ed_graph_services_state_reporting_v1_create_reporting_period_request_from_dict = EdGraphServicesStateReportingV1CreateReportingPeriodRequest.from_dict(ed_graph_services_state_reporting_v1_create_reporting_period_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


