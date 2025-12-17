# EdGraphHttpAggregatorsTenantApiControllersV2RequestsAddSeoaaRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**seoaa_id** | **str** |  | [optional] 
**education_organization_id** | **int** |  | [optional] 
**staff_classification_descriptor** | **str** |  | [optional] 
**staff_unique_id** | **str** |  | [optional] 
**begin_date** | **str** |  | [optional] 
**end_date** | **str** |  | [optional] 
**source** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v2_requests_add_seoaa_request import EdGraphHttpAggregatorsTenantApiControllersV2RequestsAddSeoaaRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV2RequestsAddSeoaaRequest from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v2_requests_add_seoaa_request_instance = EdGraphHttpAggregatorsTenantApiControllersV2RequestsAddSeoaaRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV2RequestsAddSeoaaRequest.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v2_requests_add_seoaa_request_dict = ed_graph_http_aggregators_tenant_api_controllers_v2_requests_add_seoaa_request_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV2RequestsAddSeoaaRequest from a dict
ed_graph_http_aggregators_tenant_api_controllers_v2_requests_add_seoaa_request_from_dict = EdGraphHttpAggregatorsTenantApiControllersV2RequestsAddSeoaaRequest.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v2_requests_add_seoaa_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


