# EdGraphHttpAggregatorsTenantApiServicesObservationsObservationDraftResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**form_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**data** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**observation_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_observation_draft_response import EdGraphHttpAggregatorsTenantApiServicesObservationsObservationDraftResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsObservationDraftResponse from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_observation_draft_response_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsObservationDraftResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsObservationDraftResponse.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_observation_draft_response_dict = ed_graph_http_aggregators_tenant_api_services_observations_observation_draft_response_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsObservationDraftResponse from a dict
ed_graph_http_aggregators_tenant_api_services_observations_observation_draft_response_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsObservationDraftResponse.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_observation_draft_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


