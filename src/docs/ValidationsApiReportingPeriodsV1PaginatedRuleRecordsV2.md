# ValidationsApiReportingPeriodsV1PaginatedRuleRecordsV2


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[ValidationsApiReportingPeriodsV1ValidationResultRecord]**](ValidationsApiReportingPeriodsV1ValidationResultRecord.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_paginated_rule_records_v2 import ValidationsApiReportingPeriodsV1PaginatedRuleRecordsV2

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1PaginatedRuleRecordsV2 from a JSON string
validations_api_reporting_periods_v1_paginated_rule_records_v2_instance = ValidationsApiReportingPeriodsV1PaginatedRuleRecordsV2.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1PaginatedRuleRecordsV2.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_paginated_rule_records_v2_dict = validations_api_reporting_periods_v1_paginated_rule_records_v2_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1PaginatedRuleRecordsV2 from a dict
validations_api_reporting_periods_v1_paginated_rule_records_v2_from_dict = ValidationsApiReportingPeriodsV1PaginatedRuleRecordsV2.from_dict(validations_api_reporting_periods_v1_paginated_rule_records_v2_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


