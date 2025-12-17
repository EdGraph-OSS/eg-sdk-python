# EdGraphServicesStateReportingV1PaginatedReportingPeriods


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EdGraphServicesStateReportingV1ReportingPeriodListResponse]**](EdGraphServicesStateReportingV1ReportingPeriodListResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_paginated_reporting_periods import EdGraphServicesStateReportingV1PaginatedReportingPeriods

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1PaginatedReportingPeriods from a JSON string
ed_graph_services_state_reporting_v1_paginated_reporting_periods_instance = EdGraphServicesStateReportingV1PaginatedReportingPeriods.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1PaginatedReportingPeriods.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_paginated_reporting_periods_dict = ed_graph_services_state_reporting_v1_paginated_reporting_periods_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1PaginatedReportingPeriods from a dict
ed_graph_services_state_reporting_v1_paginated_reporting_periods_from_dict = EdGraphServicesStateReportingV1PaginatedReportingPeriods.from_dict(ed_graph_services_state_reporting_v1_paginated_reporting_periods_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


