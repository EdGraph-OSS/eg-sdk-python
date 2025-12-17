# EdGraphHttpAggregatorsTenantApiServicesConnectorsExtensionsADLSGen2ConnectorProfileDTO


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**connector_type** | **str** |  | [optional] 
**connector_name** | **str** |  | [optional] 
**workspace_name** | **str** |  | [optional] 
**authentication_type** | [**AnalyticsApiADLSGen2ConnectorsV1AuthenticationType**](AnalyticsApiADLSGen2ConnectorsV1AuthenticationType.md) |  | [optional] 
**pipeline** | [**EdGraphHttpAggregatorsTenantApiServicesConnectorsExtensionsADLSGen2ConnectorProfilePipelineDTO**](EdGraphHttpAggregatorsTenantApiServicesConnectorsExtensionsADLSGen2ConnectorProfilePipelineDTO.md) |  | [optional] 
**metadata** | **object** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_connectors_extensions_adls_gen2_connector_profile_dto import EdGraphHttpAggregatorsTenantApiServicesConnectorsExtensionsADLSGen2ConnectorProfileDTO

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesConnectorsExtensionsADLSGen2ConnectorProfileDTO from a JSON string
ed_graph_http_aggregators_tenant_api_services_connectors_extensions_adls_gen2_connector_profile_dto_instance = EdGraphHttpAggregatorsTenantApiServicesConnectorsExtensionsADLSGen2ConnectorProfileDTO.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesConnectorsExtensionsADLSGen2ConnectorProfileDTO.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_connectors_extensions_adls_gen2_connector_profile_dto_dict = ed_graph_http_aggregators_tenant_api_services_connectors_extensions_adls_gen2_connector_profile_dto_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesConnectorsExtensionsADLSGen2ConnectorProfileDTO from a dict
ed_graph_http_aggregators_tenant_api_services_connectors_extensions_adls_gen2_connector_profile_dto_from_dict = EdGraphHttpAggregatorsTenantApiServicesConnectorsExtensionsADLSGen2ConnectorProfileDTO.from_dict(ed_graph_http_aggregators_tenant_api_services_connectors_extensions_adls_gen2_connector_profile_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


