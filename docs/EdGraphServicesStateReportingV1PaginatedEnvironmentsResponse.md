# EdGraphServicesStateReportingV1PaginatedEnvironmentsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EdGraphServicesStateReportingV1EnvironmentListResponse]**](EdGraphServicesStateReportingV1EnvironmentListResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_paginated_environments_response import EdGraphServicesStateReportingV1PaginatedEnvironmentsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1PaginatedEnvironmentsResponse from a JSON string
ed_graph_services_state_reporting_v1_paginated_environments_response_instance = EdGraphServicesStateReportingV1PaginatedEnvironmentsResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1PaginatedEnvironmentsResponse.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_paginated_environments_response_dict = ed_graph_services_state_reporting_v1_paginated_environments_response_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1PaginatedEnvironmentsResponse from a dict
ed_graph_services_state_reporting_v1_paginated_environments_response_from_dict = EdGraphServicesStateReportingV1PaginatedEnvironmentsResponse.from_dict(ed_graph_services_state_reporting_v1_paginated_environments_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


