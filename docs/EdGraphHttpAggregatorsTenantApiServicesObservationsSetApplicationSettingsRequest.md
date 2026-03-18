# EdGraphHttpAggregatorsTenantApiServicesObservationsSetApplicationSettingsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**forms** | [**List[EdGraphHttpAggregatorsTenantApiServicesObservationsFormConfigurationRequest]**](EdGraphHttpAggregatorsTenantApiServicesObservationsFormConfigurationRequest.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_set_application_settings_request import EdGraphHttpAggregatorsTenantApiServicesObservationsSetApplicationSettingsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsSetApplicationSettingsRequest from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_set_application_settings_request_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsSetApplicationSettingsRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsSetApplicationSettingsRequest.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_set_application_settings_request_dict = ed_graph_http_aggregators_tenant_api_services_observations_set_application_settings_request_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsSetApplicationSettingsRequest from a dict
ed_graph_http_aggregators_tenant_api_services_observations_set_application_settings_request_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsSetApplicationSettingsRequest.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_set_application_settings_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


