# EdGraphHttpAggregatorsTenantApiServicesObservationsSetRoleConfigurationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**role** | **str** |  | [optional] 
**assigned_persona_identifiers** | **List[str]** |  | [optional] 
**ignore_organization** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_set_role_configuration_request import EdGraphHttpAggregatorsTenantApiServicesObservationsSetRoleConfigurationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsSetRoleConfigurationRequest from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_set_role_configuration_request_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsSetRoleConfigurationRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsSetRoleConfigurationRequest.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_set_role_configuration_request_dict = ed_graph_http_aggregators_tenant_api_services_observations_set_role_configuration_request_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsSetRoleConfigurationRequest from a dict
ed_graph_http_aggregators_tenant_api_services_observations_set_role_configuration_request_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsSetRoleConfigurationRequest.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_set_role_configuration_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


