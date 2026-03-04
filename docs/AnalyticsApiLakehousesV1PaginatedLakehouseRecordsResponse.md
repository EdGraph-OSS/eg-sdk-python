# AnalyticsApiLakehousesV1PaginatedLakehouseRecordsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[AnalyticsApiLakehousesV1LakehouseRecord]**](AnalyticsApiLakehousesV1LakehouseRecord.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.analytics_api_lakehouses_v1_paginated_lakehouse_records_response import AnalyticsApiLakehousesV1PaginatedLakehouseRecordsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiLakehousesV1PaginatedLakehouseRecordsResponse from a JSON string
analytics_api_lakehouses_v1_paginated_lakehouse_records_response_instance = AnalyticsApiLakehousesV1PaginatedLakehouseRecordsResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiLakehousesV1PaginatedLakehouseRecordsResponse.to_json())

# convert the object into a dict
analytics_api_lakehouses_v1_paginated_lakehouse_records_response_dict = analytics_api_lakehouses_v1_paginated_lakehouse_records_response_instance.to_dict()
# create an instance of AnalyticsApiLakehousesV1PaginatedLakehouseRecordsResponse from a dict
analytics_api_lakehouses_v1_paginated_lakehouse_records_response_from_dict = AnalyticsApiLakehousesV1PaginatedLakehouseRecordsResponse.from_dict(analytics_api_lakehouses_v1_paginated_lakehouse_records_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


