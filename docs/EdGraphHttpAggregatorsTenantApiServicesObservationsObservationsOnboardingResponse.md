# EdGraphHttpAggregatorsTenantApiServicesObservationsObservationsOnboardingResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**subscription_id** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**progress_percentage** | **float** |  | [optional] 
**total_steps** | **int** |  | [optional] 
**last_completed_step** | **int** |  | [optional] 
**started_at** | **str** |  | [optional] 
**completed_at** | **str** |  | [optional] 
**steps** | [**List[EdGraphHttpAggregatorsTenantApiServicesObservationsObservationsOnboardingStepResponse]**](EdGraphHttpAggregatorsTenantApiServicesObservationsObservationsOnboardingStepResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_observations_onboarding_response import EdGraphHttpAggregatorsTenantApiServicesObservationsObservationsOnboardingResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsObservationsOnboardingResponse from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_observations_onboarding_response_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsObservationsOnboardingResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsObservationsOnboardingResponse.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_observations_onboarding_response_dict = ed_graph_http_aggregators_tenant_api_services_observations_observations_onboarding_response_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsObservationsOnboardingResponse from a dict
ed_graph_http_aggregators_tenant_api_services_observations_observations_onboarding_response_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsObservationsOnboardingResponse.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_observations_onboarding_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


