# EdGraphHttpAggregatorsTenantApiControllersV2RequestsUpdateSeoaaRequest


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

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v2_requests_update_seoaa_request import EdGraphHttpAggregatorsTenantApiControllersV2RequestsUpdateSeoaaRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV2RequestsUpdateSeoaaRequest from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v2_requests_update_seoaa_request_instance = EdGraphHttpAggregatorsTenantApiControllersV2RequestsUpdateSeoaaRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV2RequestsUpdateSeoaaRequest.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v2_requests_update_seoaa_request_dict = ed_graph_http_aggregators_tenant_api_controllers_v2_requests_update_seoaa_request_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV2RequestsUpdateSeoaaRequest from a dict
ed_graph_http_aggregators_tenant_api_controllers_v2_requests_update_seoaa_request_from_dict = EdGraphHttpAggregatorsTenantApiControllersV2RequestsUpdateSeoaaRequest.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v2_requests_update_seoaa_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


