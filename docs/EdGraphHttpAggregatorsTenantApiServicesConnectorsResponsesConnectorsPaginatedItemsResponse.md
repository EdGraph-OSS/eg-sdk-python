# EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorsPaginatedItemsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**count** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**page_index** | **int** |  | [optional] 
**data** | [**List[EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesMappedConnectorListResponse]**](EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesMappedConnectorListResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_connectors_responses_connectors_paginated_items_response import EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorsPaginatedItemsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorsPaginatedItemsResponse from a JSON string
ed_graph_http_aggregators_tenant_api_services_connectors_responses_connectors_paginated_items_response_instance = EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorsPaginatedItemsResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorsPaginatedItemsResponse.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_connectors_responses_connectors_paginated_items_response_dict = ed_graph_http_aggregators_tenant_api_services_connectors_responses_connectors_paginated_items_response_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorsPaginatedItemsResponse from a dict
ed_graph_http_aggregators_tenant_api_services_connectors_responses_connectors_paginated_items_response_from_dict = EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesConnectorsPaginatedItemsResponse.from_dict(ed_graph_http_aggregators_tenant_api_services_connectors_responses_connectors_paginated_items_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


