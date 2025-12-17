# EdGraphServicesStateReportingV1UpdateReportingPeriodBulkRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**reporting_periods** | [**List[EdGraphServicesStateReportingV1UpdateReportingPeriodBulkRequestTypesReportingPeriod]**](EdGraphServicesStateReportingV1UpdateReportingPeriodBulkRequestTypesReportingPeriod.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_update_reporting_period_bulk_request import EdGraphServicesStateReportingV1UpdateReportingPeriodBulkRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1UpdateReportingPeriodBulkRequest from a JSON string
ed_graph_services_state_reporting_v1_update_reporting_period_bulk_request_instance = EdGraphServicesStateReportingV1UpdateReportingPeriodBulkRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1UpdateReportingPeriodBulkRequest.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_update_reporting_period_bulk_request_dict = ed_graph_services_state_reporting_v1_update_reporting_period_bulk_request_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1UpdateReportingPeriodBulkRequest from a dict
ed_graph_services_state_reporting_v1_update_reporting_period_bulk_request_from_dict = EdGraphServicesStateReportingV1UpdateReportingPeriodBulkRequest.from_dict(ed_graph_services_state_reporting_v1_update_reporting_period_bulk_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


