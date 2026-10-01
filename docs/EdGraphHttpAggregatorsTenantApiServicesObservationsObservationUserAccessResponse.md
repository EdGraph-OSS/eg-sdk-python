# EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserAccessResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**access_scope_type** | **str** |  | [optional] 
**available_organizations** | **List[str]** |  | [optional] 
**available_persona_identifiers** | **List[str]** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_observation_user_access_response import EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserAccessResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserAccessResponse from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_observation_user_access_response_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserAccessResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserAccessResponse.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_observation_user_access_response_dict = ed_graph_http_aggregators_tenant_api_services_observations_observation_user_access_response_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserAccessResponse from a dict
ed_graph_http_aggregators_tenant_api_services_observations_observation_user_access_response_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserAccessResponse.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_observation_user_access_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


