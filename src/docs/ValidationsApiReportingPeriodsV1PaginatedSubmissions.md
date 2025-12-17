# ValidationsApiReportingPeriodsV1PaginatedSubmissions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[ValidationsApiReportingPeriodsV1SubmissionListResponse]**](ValidationsApiReportingPeriodsV1SubmissionListResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_paginated_submissions import ValidationsApiReportingPeriodsV1PaginatedSubmissions

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1PaginatedSubmissions from a JSON string
validations_api_reporting_periods_v1_paginated_submissions_instance = ValidationsApiReportingPeriodsV1PaginatedSubmissions.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1PaginatedSubmissions.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_paginated_submissions_dict = validations_api_reporting_periods_v1_paginated_submissions_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1PaginatedSubmissions from a dict
validations_api_reporting_periods_v1_paginated_submissions_from_dict = ValidationsApiReportingPeriodsV1PaginatedSubmissions.from_dict(validations_api_reporting_periods_v1_paginated_submissions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


