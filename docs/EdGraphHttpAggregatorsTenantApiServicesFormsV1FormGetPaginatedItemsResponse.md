# EdGraphHttpAggregatorsTenantApiServicesFormsV1FormGetPaginatedItemsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**data** | [**List[EdGraphHttpAggregatorsTenantApiServicesFormsV1Form]**](EdGraphHttpAggregatorsTenantApiServicesFormsV1Form.md) |  | [optional] 
**count** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_forms_v1_form_get_paginated_items_response import EdGraphHttpAggregatorsTenantApiServicesFormsV1FormGetPaginatedItemsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesFormsV1FormGetPaginatedItemsResponse from a JSON string
ed_graph_http_aggregators_tenant_api_services_forms_v1_form_get_paginated_items_response_instance = EdGraphHttpAggregatorsTenantApiServicesFormsV1FormGetPaginatedItemsResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesFormsV1FormGetPaginatedItemsResponse.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_forms_v1_form_get_paginated_items_response_dict = ed_graph_http_aggregators_tenant_api_services_forms_v1_form_get_paginated_items_response_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesFormsV1FormGetPaginatedItemsResponse from a dict
ed_graph_http_aggregators_tenant_api_services_forms_v1_form_get_paginated_items_response_from_dict = EdGraphHttpAggregatorsTenantApiServicesFormsV1FormGetPaginatedItemsResponse.from_dict(ed_graph_http_aggregators_tenant_api_services_forms_v1_form_get_paginated_items_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


