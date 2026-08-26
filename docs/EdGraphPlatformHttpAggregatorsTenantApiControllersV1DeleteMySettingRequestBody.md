# EdGraphPlatformHttpAggregatorsTenantApiControllersV1DeleteMySettingRequestBody


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**setting_type_id** | **UUID** |  | [optional] 
**provider** | **str** |  | [optional] 
**application_id** | **UUID** |  | [optional] 
**reason** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_delete_my_setting_request_body import EdGraphPlatformHttpAggregatorsTenantApiControllersV1DeleteMySettingRequestBody

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1DeleteMySettingRequestBody from a JSON string
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_delete_my_setting_request_body_instance = EdGraphPlatformHttpAggregatorsTenantApiControllersV1DeleteMySettingRequestBody.from_json(json)
# print the JSON string representation of the object
print(EdGraphPlatformHttpAggregatorsTenantApiControllersV1DeleteMySettingRequestBody.to_json())

# convert the object into a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_delete_my_setting_request_body_dict = ed_graph_platform_http_aggregators_tenant_api_controllers_v1_delete_my_setting_request_body_instance.to_dict()
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1DeleteMySettingRequestBody from a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_delete_my_setting_request_body_from_dict = EdGraphPlatformHttpAggregatorsTenantApiControllersV1DeleteMySettingRequestBody.from_dict(ed_graph_platform_http_aggregators_tenant_api_controllers_v1_delete_my_setting_request_body_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


