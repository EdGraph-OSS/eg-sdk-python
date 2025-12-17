# ValidationsApiReportingPeriodsV1PaginatedReportingPeriods


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[ValidationsApiReportingPeriodsV1ReportingPeriodDto]**](ValidationsApiReportingPeriodsV1ReportingPeriodDto.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_paginated_reporting_periods import ValidationsApiReportingPeriodsV1PaginatedReportingPeriods

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1PaginatedReportingPeriods from a JSON string
validations_api_reporting_periods_v1_paginated_reporting_periods_instance = ValidationsApiReportingPeriodsV1PaginatedReportingPeriods.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1PaginatedReportingPeriods.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_paginated_reporting_periods_dict = validations_api_reporting_periods_v1_paginated_reporting_periods_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1PaginatedReportingPeriods from a dict
validations_api_reporting_periods_v1_paginated_reporting_periods_from_dict = ValidationsApiReportingPeriodsV1PaginatedReportingPeriods.from_dict(validations_api_reporting_periods_v1_paginated_reporting_periods_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


