# EdGraphHttpAggregatorsTenantApiServicesObservationsGetCampusesWithEvalueesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EdGraphHttpAggregatorsTenantApiServicesObservationsCampusWithEvalueesResponse]**](EdGraphHttpAggregatorsTenantApiServicesObservationsCampusWithEvalueesResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_get_campuses_with_evaluees_response import EdGraphHttpAggregatorsTenantApiServicesObservationsGetCampusesWithEvalueesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsGetCampusesWithEvalueesResponse from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_get_campuses_with_evaluees_response_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsGetCampusesWithEvalueesResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsGetCampusesWithEvalueesResponse.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_get_campuses_with_evaluees_response_dict = ed_graph_http_aggregators_tenant_api_services_observations_get_campuses_with_evaluees_response_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsGetCampusesWithEvalueesResponse from a dict
ed_graph_http_aggregators_tenant_api_services_observations_get_campuses_with_evaluees_response_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsGetCampusesWithEvalueesResponse.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_get_campuses_with_evaluees_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


