# EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesMappedConnectorListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**connector_name** | **str** |  | [optional] 
**connector_type** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**properties** | **object** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_connectors_responses_mapped_connector_list_response import EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesMappedConnectorListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesMappedConnectorListResponse from a JSON string
ed_graph_http_aggregators_tenant_api_services_connectors_responses_mapped_connector_list_response_instance = EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesMappedConnectorListResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesMappedConnectorListResponse.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_connectors_responses_mapped_connector_list_response_dict = ed_graph_http_aggregators_tenant_api_services_connectors_responses_mapped_connector_list_response_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesMappedConnectorListResponse from a dict
ed_graph_http_aggregators_tenant_api_services_connectors_responses_mapped_connector_list_response_from_dict = EdGraphHttpAggregatorsTenantApiServicesConnectorsResponsesMappedConnectorListResponse.from_dict(ed_graph_http_aggregators_tenant_api_services_connectors_responses_mapped_connector_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


