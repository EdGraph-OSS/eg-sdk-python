# ValidationsApiReportingPeriodsV1PaginatedRecordsTypesReportingPeriodRecords


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**rule** | [**ValidationsApiReportingPeriodsV1PaginatedRecordsTypesReportingPeriodRecordsTypesRule**](ValidationsApiReportingPeriodsV1PaginatedRecordsTypesReportingPeriodRecordsTypesRule.md) |  | [optional] 
**records** | [**List[ValidationsApiReportingPeriodsV1ValidationResultRecord]**](ValidationsApiReportingPeriodsV1ValidationResultRecord.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_paginated_records_types_reporting_period_records import ValidationsApiReportingPeriodsV1PaginatedRecordsTypesReportingPeriodRecords

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1PaginatedRecordsTypesReportingPeriodRecords from a JSON string
validations_api_reporting_periods_v1_paginated_records_types_reporting_period_records_instance = ValidationsApiReportingPeriodsV1PaginatedRecordsTypesReportingPeriodRecords.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1PaginatedRecordsTypesReportingPeriodRecords.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_paginated_records_types_reporting_period_records_dict = validations_api_reporting_periods_v1_paginated_records_types_reporting_period_records_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1PaginatedRecordsTypesReportingPeriodRecords from a dict
validations_api_reporting_periods_v1_paginated_records_types_reporting_period_records_from_dict = ValidationsApiReportingPeriodsV1PaginatedRecordsTypesReportingPeriodRecords.from_dict(validations_api_reporting_periods_v1_paginated_records_types_reporting_period_records_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


