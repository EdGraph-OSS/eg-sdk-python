# EdGraphHttpAggregatorsTenantApiServicesObservationsGetStaffClassificationSettingsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**namespaces** | [**List[EdGraphHttpAggregatorsTenantApiServicesObservationsStaffClassificationNamespaceConfiguration]**](EdGraphHttpAggregatorsTenantApiServicesObservationsStaffClassificationNamespaceConfiguration.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_get_staff_classification_settings_response import EdGraphHttpAggregatorsTenantApiServicesObservationsGetStaffClassificationSettingsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsGetStaffClassificationSettingsResponse from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_get_staff_classification_settings_response_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsGetStaffClassificationSettingsResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsGetStaffClassificationSettingsResponse.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_get_staff_classification_settings_response_dict = ed_graph_http_aggregators_tenant_api_services_observations_get_staff_classification_settings_response_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsGetStaffClassificationSettingsResponse from a dict
ed_graph_http_aggregators_tenant_api_services_observations_get_staff_classification_settings_response_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsGetStaffClassificationSettingsResponse.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_get_staff_classification_settings_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


