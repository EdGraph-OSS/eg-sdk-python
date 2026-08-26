# EdGraphHttpAggregatorsTenantApiControllersV2DeleteClientSettingRequestBody


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**setting_type_id** | **UUID** |  | [optional] 
**provider** | **str** |  | [optional] 
**application_id** | **UUID** |  | [optional] 
**reason** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v2_delete_client_setting_request_body import EdGraphHttpAggregatorsTenantApiControllersV2DeleteClientSettingRequestBody

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV2DeleteClientSettingRequestBody from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v2_delete_client_setting_request_body_instance = EdGraphHttpAggregatorsTenantApiControllersV2DeleteClientSettingRequestBody.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV2DeleteClientSettingRequestBody.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v2_delete_client_setting_request_body_dict = ed_graph_http_aggregators_tenant_api_controllers_v2_delete_client_setting_request_body_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV2DeleteClientSettingRequestBody from a dict
ed_graph_http_aggregators_tenant_api_controllers_v2_delete_client_setting_request_body_from_dict = EdGraphHttpAggregatorsTenantApiControllersV2DeleteClientSettingRequestBody.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v2_delete_client_setting_request_body_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


