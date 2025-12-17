# EdGraphServicesStateReportingV1PaginatedCategories


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EdGraphServicesStateReportingV1Category]**](EdGraphServicesStateReportingV1Category.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_paginated_categories import EdGraphServicesStateReportingV1PaginatedCategories

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1PaginatedCategories from a JSON string
ed_graph_services_state_reporting_v1_paginated_categories_instance = EdGraphServicesStateReportingV1PaginatedCategories.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1PaginatedCategories.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_paginated_categories_dict = ed_graph_services_state_reporting_v1_paginated_categories_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1PaginatedCategories from a dict
ed_graph_services_state_reporting_v1_paginated_categories_from_dict = EdGraphServicesStateReportingV1PaginatedCategories.from_dict(ed_graph_services_state_reporting_v1_paginated_categories_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


