# EdGraphServicesStateReportingV1PaginatedRecords


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EdGraphServicesStateReportingV1PaginatedRecordsTypesReportingPeriodRecords]**](EdGraphServicesStateReportingV1PaginatedRecordsTypesReportingPeriodRecords.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_paginated_records import EdGraphServicesStateReportingV1PaginatedRecords

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1PaginatedRecords from a JSON string
ed_graph_services_state_reporting_v1_paginated_records_instance = EdGraphServicesStateReportingV1PaginatedRecords.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1PaginatedRecords.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_paginated_records_dict = ed_graph_services_state_reporting_v1_paginated_records_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1PaginatedRecords from a dict
ed_graph_services_state_reporting_v1_paginated_records_from_dict = EdGraphServicesStateReportingV1PaginatedRecords.from_dict(ed_graph_services_state_reporting_v1_paginated_records_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


