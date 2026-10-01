# EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserResponse

ObservationAccess is null only when Identity has no ObservationAccessScope bulk result for that user  (e.g. the user has no tenant membership matching the request's tenantId).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**source** | **str** |  | [optional] 
**instructional_insights_role** | **str** |  | [optional] 
**seoaas** | [**List[EdGraphHttpAggregatorsTenantApiServicesObservationsSeoaaResponse]**](EdGraphHttpAggregatorsTenantApiServicesObservationsSeoaaResponse.md) |  | [optional] 
**observation_access** | [**EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserAccessResponse**](EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserAccessResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_observation_user_response import EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserResponse from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_observation_user_response_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserResponse.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_observation_user_response_dict = ed_graph_http_aggregators_tenant_api_services_observations_observation_user_response_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserResponse from a dict
ed_graph_http_aggregators_tenant_api_services_observations_observation_user_response_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsObservationUserResponse.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_observation_user_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


