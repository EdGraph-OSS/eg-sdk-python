# EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationSubmissionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**form_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**current_step** | **int** |  | [optional] 
**data** | **str** |  | [optional] 
**observation_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_create_observation_submission_request import EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationSubmissionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationSubmissionRequest from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_create_observation_submission_request_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationSubmissionRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationSubmissionRequest.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_create_observation_submission_request_dict = ed_graph_http_aggregators_tenant_api_services_observations_create_observation_submission_request_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationSubmissionRequest from a dict
ed_graph_http_aggregators_tenant_api_services_observations_create_observation_submission_request_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsCreateObservationSubmissionRequest.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_create_observation_submission_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


