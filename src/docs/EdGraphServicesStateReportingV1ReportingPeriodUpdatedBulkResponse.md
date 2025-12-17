# EdGraphServicesStateReportingV1ReportingPeriodUpdatedBulkResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**reporting_period_ids** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_updated_bulk_response import EdGraphServicesStateReportingV1ReportingPeriodUpdatedBulkResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodUpdatedBulkResponse from a JSON string
ed_graph_services_state_reporting_v1_reporting_period_updated_bulk_response_instance = EdGraphServicesStateReportingV1ReportingPeriodUpdatedBulkResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1ReportingPeriodUpdatedBulkResponse.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_reporting_period_updated_bulk_response_dict = ed_graph_services_state_reporting_v1_reporting_period_updated_bulk_response_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodUpdatedBulkResponse from a dict
ed_graph_services_state_reporting_v1_reporting_period_updated_bulk_response_from_dict = EdGraphServicesStateReportingV1ReportingPeriodUpdatedBulkResponse.from_dict(ed_graph_services_state_reporting_v1_reporting_period_updated_bulk_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


