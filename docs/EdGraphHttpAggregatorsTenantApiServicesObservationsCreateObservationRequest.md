# EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**observation_date** | **str** |  | [optional] 
**campus** | **str** |  | [optional] 
**observer_id** | **str** |  | [optional] 
**evaluee_id** | **str** |  | [optional] 
**form_id** | **str** |  | [optional] 
**form_version** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_create_observation_request import EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationRequest from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_create_observation_request_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationRequest.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_create_observation_request_dict = ed_graph_http_aggregators_tenant_api_services_observations_create_observation_request_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationRequest from a dict
ed_graph_http_aggregators_tenant_api_services_observations_create_observation_request_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationRequest.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_create_observation_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


