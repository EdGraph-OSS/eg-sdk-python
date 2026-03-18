# EdGraphHttpAggregatorsTenantApiServicesObservationsObservationProfileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**campus** | **str** |  | [optional] 
**observer_id** | **str** |  | [optional] 
**observer_name** | **str** |  | [optional] 
**evaluee_id** | **str** |  | [optional] 
**evaluee_name** | **str** |  | [optional] 
**form_id** | **str** |  | [optional] 
**form_version** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**var_class** | **str** |  | [optional] 
**observation_date** | **str** |  | [optional] 
**submission_date** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_observation_profile_response import EdGraphHttpAggregatorsTenantApiServicesObservationsObservationProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsObservationProfileResponse from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_observation_profile_response_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsObservationProfileResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsObservationProfileResponse.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_observation_profile_response_dict = ed_graph_http_aggregators_tenant_api_services_observations_observation_profile_response_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsObservationProfileResponse from a dict
ed_graph_http_aggregators_tenant_api_services_observations_observation_profile_response_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsObservationProfileResponse.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_observation_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


