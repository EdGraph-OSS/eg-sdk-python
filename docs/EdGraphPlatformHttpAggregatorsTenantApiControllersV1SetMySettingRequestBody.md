# EdGraphPlatformHttpAggregatorsTenantApiControllersV1SetMySettingRequestBody


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**setting_id** | **UUID** |  | [optional] 
**setting_type_id** | **UUID** |  | [optional] 
**provider** | **str** |  | [optional] 
**code** | **str** |  | [optional] 
**application_id** | **UUID** |  | [optional] 
**value** | **object** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_set_my_setting_request_body import EdGraphPlatformHttpAggregatorsTenantApiControllersV1SetMySettingRequestBody

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1SetMySettingRequestBody from a JSON string
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_set_my_setting_request_body_instance = EdGraphPlatformHttpAggregatorsTenantApiControllersV1SetMySettingRequestBody.from_json(json)
# print the JSON string representation of the object
print(EdGraphPlatformHttpAggregatorsTenantApiControllersV1SetMySettingRequestBody.to_json())

# convert the object into a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_set_my_setting_request_body_dict = ed_graph_platform_http_aggregators_tenant_api_controllers_v1_set_my_setting_request_body_instance.to_dict()
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1SetMySettingRequestBody from a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_set_my_setting_request_body_from_dict = EdGraphPlatformHttpAggregatorsTenantApiControllersV1SetMySettingRequestBody.from_dict(ed_graph_platform_http_aggregators_tenant_api_controllers_v1_set_my_setting_request_body_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


