# EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**rule_id** | **str** |  | [optional] 
**record_id** | **str** |  | [optional] 
**exclude_from_post** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_request import EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagRequest from a JSON string
ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_request_instance = EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagRequest.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_request_dict = ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_request_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagRequest from a dict
ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_request_from_dict = EdGraphServicesStateReportingV1SetReportingPeriodRuleRecordPostFlagRequest.from_dict(ed_graph_services_state_reporting_v1_set_reporting_period_rule_record_post_flag_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


