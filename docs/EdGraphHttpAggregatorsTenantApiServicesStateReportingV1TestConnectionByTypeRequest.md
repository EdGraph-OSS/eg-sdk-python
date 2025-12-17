# EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionByTypeRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**type** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**server** | **str** |  | [optional] 
**username** | **str** |  | [optional] 
**database** | **str** |  | [optional] 
**password** | **str** |  | [optional] 
**auth_url** | **str** |  | [optional] 
**resources_url** | **str** |  | [optional] 
**api_key** | **str** |  | [optional] 
**api_secret** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_test_connection_by_type_request import EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionByTypeRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionByTypeRequest from a JSON string
ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_test_connection_by_type_request_instance = EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionByTypeRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionByTypeRequest.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_test_connection_by_type_request_dict = ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_test_connection_by_type_request_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionByTypeRequest from a dict
ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_test_connection_by_type_request_from_dict = EdGraphHttpAggregatorsTenantApiServicesStateReportingV1TestConnectionByTypeRequest.from_dict(ed_graph_http_aggregators_tenant_api_services_state_reporting_v1_test_connection_by_type_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


