# EdGraphServicesStateReportingV1PaginatedSubCategories


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EdGraphServicesStateReportingV1SubCategory]**](EdGraphServicesStateReportingV1SubCategory.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_paginated_sub_categories import EdGraphServicesStateReportingV1PaginatedSubCategories

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1PaginatedSubCategories from a JSON string
ed_graph_services_state_reporting_v1_paginated_sub_categories_instance = EdGraphServicesStateReportingV1PaginatedSubCategories.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1PaginatedSubCategories.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_paginated_sub_categories_dict = ed_graph_services_state_reporting_v1_paginated_sub_categories_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1PaginatedSubCategories from a dict
ed_graph_services_state_reporting_v1_paginated_sub_categories_from_dict = EdGraphServicesStateReportingV1PaginatedSubCategories.from_dict(ed_graph_services_state_reporting_v1_paginated_sub_categories_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


