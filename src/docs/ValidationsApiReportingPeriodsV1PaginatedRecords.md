# ValidationsApiReportingPeriodsV1PaginatedRecords


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[ValidationsApiReportingPeriodsV1PaginatedRecordsTypesReportingPeriodRecords]**](ValidationsApiReportingPeriodsV1PaginatedRecordsTypesReportingPeriodRecords.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_paginated_records import ValidationsApiReportingPeriodsV1PaginatedRecords

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1PaginatedRecords from a JSON string
validations_api_reporting_periods_v1_paginated_records_instance = ValidationsApiReportingPeriodsV1PaginatedRecords.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1PaginatedRecords.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_paginated_records_dict = validations_api_reporting_periods_v1_paginated_records_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1PaginatedRecords from a dict
validations_api_reporting_periods_v1_paginated_records_from_dict = ValidationsApiReportingPeriodsV1PaginatedRecords.from_dict(validations_api_reporting_periods_v1_paginated_records_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


