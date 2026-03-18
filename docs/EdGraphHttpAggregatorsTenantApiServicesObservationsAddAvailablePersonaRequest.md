# EdGraphHttpAggregatorsTenantApiServicesObservationsAddAvailablePersonaRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**identifier** | **str** |  | [optional] 
**is_default** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_add_available_persona_request import EdGraphHttpAggregatorsTenantApiServicesObservationsAddAvailablePersonaRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsAddAvailablePersonaRequest from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_add_available_persona_request_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsAddAvailablePersonaRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsAddAvailablePersonaRequest.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_add_available_persona_request_dict = ed_graph_http_aggregators_tenant_api_services_observations_add_available_persona_request_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsAddAvailablePersonaRequest from a dict
ed_graph_http_aggregators_tenant_api_services_observations_add_available_persona_request_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsAddAvailablePersonaRequest.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_add_available_persona_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


