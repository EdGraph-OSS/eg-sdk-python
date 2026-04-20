# EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**observation_id** | **str** |  | [optional] 
**observation_date** | **str** |  | [optional] 
**campus** | **str** |  | [optional] 
**observer_id** | **str** |  | [optional] 
**evaluee_id** | **str** |  | [optional] 
**form_id** | **str** |  | [optional] 
**form_version** | **str** |  | [optional] 
**campus_class_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_update_observation_request import EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationRequest from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_update_observation_request_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationRequest.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_update_observation_request_dict = ed_graph_http_aggregators_tenant_api_services_observations_update_observation_request_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationRequest from a dict
ed_graph_http_aggregators_tenant_api_services_observations_update_observation_request_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsUpdateObservationRequest.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_update_observation_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


