# EdGraphHttpAggregatorsTenantApiServicesInstancesInstanceResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**instance_id** | **str** |  | [optional] 
**instance_name** | **str** |  | [optional] 
**instance_type** | **str** |  | [optional] 
**connection_type** | **str** |  | [optional] 
**provider** | **str** |  | [optional] 
**school_years** | **List[int]** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**is_default** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_instances_instance_response import EdGraphHttpAggregatorsTenantApiServicesInstancesInstanceResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesInstancesInstanceResponse from a JSON string
ed_graph_http_aggregators_tenant_api_services_instances_instance_response_instance = EdGraphHttpAggregatorsTenantApiServicesInstancesInstanceResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesInstancesInstanceResponse.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_instances_instance_response_dict = ed_graph_http_aggregators_tenant_api_services_instances_instance_response_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesInstancesInstanceResponse from a dict
ed_graph_http_aggregators_tenant_api_services_instances_instance_response_from_dict = EdGraphHttpAggregatorsTenantApiServicesInstancesInstanceResponse.from_dict(ed_graph_http_aggregators_tenant_api_services_instances_instance_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


