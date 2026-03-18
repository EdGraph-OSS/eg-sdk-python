# EdGraphHttpAggregatorsTenantApiServicesObservationsGetApplicationSettingsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**forms** | [**List[EdGraphHttpAggregatorsTenantApiServicesObservationsFormConfigurationResponse]**](EdGraphHttpAggregatorsTenantApiServicesObservationsFormConfigurationResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_get_application_settings_response import EdGraphHttpAggregatorsTenantApiServicesObservationsGetApplicationSettingsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsGetApplicationSettingsResponse from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_get_application_settings_response_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsGetApplicationSettingsResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsGetApplicationSettingsResponse.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_get_application_settings_response_dict = ed_graph_http_aggregators_tenant_api_services_observations_get_application_settings_response_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsGetApplicationSettingsResponse from a dict
ed_graph_http_aggregators_tenant_api_services_observations_get_application_settings_response_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsGetApplicationSettingsResponse.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_get_application_settings_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


