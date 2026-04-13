# EdGraphHttpAggregatorsTenantApiServicesObservationsFormResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**version** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**source** | **str** |  | [optional] 
**image** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_form_response import EdGraphHttpAggregatorsTenantApiServicesObservationsFormResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsFormResponse from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_form_response_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsFormResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsFormResponse.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_form_response_dict = ed_graph_http_aggregators_tenant_api_services_observations_form_response_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsFormResponse from a dict
ed_graph_http_aggregators_tenant_api_services_observations_form_response_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsFormResponse.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_form_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


