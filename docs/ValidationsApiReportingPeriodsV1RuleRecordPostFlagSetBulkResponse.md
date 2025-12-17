# ValidationsApiReportingPeriodsV1RuleRecordPostFlagSetBulkResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**rule_id** | **str** |  | [optional] 
**record_ids** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_rule_record_post_flag_set_bulk_response import ValidationsApiReportingPeriodsV1RuleRecordPostFlagSetBulkResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1RuleRecordPostFlagSetBulkResponse from a JSON string
validations_api_reporting_periods_v1_rule_record_post_flag_set_bulk_response_instance = ValidationsApiReportingPeriodsV1RuleRecordPostFlagSetBulkResponse.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1RuleRecordPostFlagSetBulkResponse.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_rule_record_post_flag_set_bulk_response_dict = validations_api_reporting_periods_v1_rule_record_post_flag_set_bulk_response_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1RuleRecordPostFlagSetBulkResponse from a dict
validations_api_reporting_periods_v1_rule_record_post_flag_set_bulk_response_from_dict = ValidationsApiReportingPeriodsV1RuleRecordPostFlagSetBulkResponse.from_dict(validations_api_reporting_periods_v1_rule_record_post_flag_set_bulk_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


