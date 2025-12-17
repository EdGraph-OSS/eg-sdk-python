# EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagBulkRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**rule_id** | **str** |  | [optional] 
**records** | [**List[EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagBulkRequestTypesRecord]**](EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagBulkRequestTypesRecord.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_bulk_request import EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagBulkRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagBulkRequest from a JSON string
ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_bulk_request_instance = EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagBulkRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagBulkRequest.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_bulk_request_dict = ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_bulk_request_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagBulkRequest from a dict
ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_bulk_request_from_dict = EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagBulkRequest.from_dict(ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_bulk_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


