# EdGraphHttpAggregatorsTenantApiControllersV2CreateTenantSettingRequestBody


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
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v2_create_tenant_setting_request_body import EdGraphHttpAggregatorsTenantApiControllersV2CreateTenantSettingRequestBody

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV2CreateTenantSettingRequestBody from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v2_create_tenant_setting_request_body_instance = EdGraphHttpAggregatorsTenantApiControllersV2CreateTenantSettingRequestBody.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV2CreateTenantSettingRequestBody.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v2_create_tenant_setting_request_body_dict = ed_graph_http_aggregators_tenant_api_controllers_v2_create_tenant_setting_request_body_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV2CreateTenantSettingRequestBody from a dict
ed_graph_http_aggregators_tenant_api_controllers_v2_create_tenant_setting_request_body_from_dict = EdGraphHttpAggregatorsTenantApiControllersV2CreateTenantSettingRequestBody.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v2_create_tenant_setting_request_body_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


