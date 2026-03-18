# EdGraphHttpAggregatorsTenantApiServicesObservationsFormConfigurationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**form_id** | **str** |  | [optional] 
**versions** | [**List[EdGraphHttpAggregatorsTenantApiServicesObservationsFormVersionConfigurationRequest]**](EdGraphHttpAggregatorsTenantApiServicesObservationsFormVersionConfigurationRequest.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_form_configuration_request import EdGraphHttpAggregatorsTenantApiServicesObservationsFormConfigurationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsFormConfigurationRequest from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_form_configuration_request_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsFormConfigurationRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsFormConfigurationRequest.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_form_configuration_request_dict = ed_graph_http_aggregators_tenant_api_services_observations_form_configuration_request_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsFormConfigurationRequest from a dict
ed_graph_http_aggregators_tenant_api_services_observations_form_configuration_request_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsFormConfigurationRequest.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_form_configuration_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


