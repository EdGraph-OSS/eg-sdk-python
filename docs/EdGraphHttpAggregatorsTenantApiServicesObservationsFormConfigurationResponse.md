# EdGraphHttpAggregatorsTenantApiServicesObservationsFormConfigurationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**form_id** | **str** |  | [optional] 
**versions** | [**List[EdGraphHttpAggregatorsTenantApiServicesObservationsFormVersionConfigurationResponse]**](EdGraphHttpAggregatorsTenantApiServicesObservationsFormVersionConfigurationResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_form_configuration_response import EdGraphHttpAggregatorsTenantApiServicesObservationsFormConfigurationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsFormConfigurationResponse from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_form_configuration_response_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsFormConfigurationResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsFormConfigurationResponse.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_form_configuration_response_dict = ed_graph_http_aggregators_tenant_api_services_observations_form_configuration_response_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsFormConfigurationResponse from a dict
ed_graph_http_aggregators_tenant_api_services_observations_form_configuration_response_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsFormConfigurationResponse.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_form_configuration_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


