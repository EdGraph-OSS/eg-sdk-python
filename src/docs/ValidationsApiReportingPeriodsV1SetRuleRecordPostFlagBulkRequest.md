# ValidationsApiReportingPeriodsV1SetRuleRecordPostFlagBulkRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**rule_id** | **str** |  | [optional] 
**records** | [**List[ValidationsApiReportingPeriodsV1SetRuleRecordPostFlagBulkRequestTypesRecord]**](ValidationsApiReportingPeriodsV1SetRuleRecordPostFlagBulkRequestTypesRecord.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_set_rule_record_post_flag_bulk_request import ValidationsApiReportingPeriodsV1SetRuleRecordPostFlagBulkRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1SetRuleRecordPostFlagBulkRequest from a JSON string
validations_api_reporting_periods_v1_set_rule_record_post_flag_bulk_request_instance = ValidationsApiReportingPeriodsV1SetRuleRecordPostFlagBulkRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1SetRuleRecordPostFlagBulkRequest.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_set_rule_record_post_flag_bulk_request_dict = validations_api_reporting_periods_v1_set_rule_record_post_flag_bulk_request_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1SetRuleRecordPostFlagBulkRequest from a dict
validations_api_reporting_periods_v1_set_rule_record_post_flag_bulk_request_from_dict = ValidationsApiReportingPeriodsV1SetRuleRecordPostFlagBulkRequest.from_dict(validations_api_reporting_periods_v1_set_rule_record_post_flag_bulk_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


