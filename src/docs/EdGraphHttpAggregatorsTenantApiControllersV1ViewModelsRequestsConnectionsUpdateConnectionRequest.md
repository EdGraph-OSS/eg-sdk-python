# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsUpdateConnectionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**connection_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**provider_id** | **str** |  | [optional] 
**connection_type_id** | **str** |  | [optional] 
**connection_metadata** | [**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsConnectionMetadata]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsConnectionMetadata.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_update_connection_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsUpdateConnectionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsUpdateConnectionRequest from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_update_connection_request_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsUpdateConnectionRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsUpdateConnectionRequest.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_update_connection_request_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_update_connection_request_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsUpdateConnectionRequest from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_update_connection_request_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsConnectionsUpdateConnectionRequest.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_connections_update_connection_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


