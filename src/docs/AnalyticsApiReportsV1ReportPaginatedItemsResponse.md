# AnalyticsApiReportsV1ReportPaginatedItemsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[AnalyticsApiReportsV1AnalyticsReport]**](AnalyticsApiReportsV1AnalyticsReport.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.analytics_api_reports_v1_report_paginated_items_response import AnalyticsApiReportsV1ReportPaginatedItemsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiReportsV1ReportPaginatedItemsResponse from a JSON string
analytics_api_reports_v1_report_paginated_items_response_instance = AnalyticsApiReportsV1ReportPaginatedItemsResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiReportsV1ReportPaginatedItemsResponse.to_json())

# convert the object into a dict
analytics_api_reports_v1_report_paginated_items_response_dict = analytics_api_reports_v1_report_paginated_items_response_instance.to_dict()
# create an instance of AnalyticsApiReportsV1ReportPaginatedItemsResponse from a dict
analytics_api_reports_v1_report_paginated_items_response_from_dict = AnalyticsApiReportsV1ReportPaginatedItemsResponse.from_dict(analytics_api_reports_v1_report_paginated_items_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


