# TenantApiTenantV1SetAppSettingsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**code** | **str** |  | [optional] 
**data** | **str** |  | [optional] 
**data_type** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_set_app_settings_request import TenantApiTenantV1SetAppSettingsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1SetAppSettingsRequest from a JSON string
tenant_api_tenant_v1_set_app_settings_request_instance = TenantApiTenantV1SetAppSettingsRequest.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1SetAppSettingsRequest.to_json())

# convert the object into a dict
tenant_api_tenant_v1_set_app_settings_request_dict = tenant_api_tenant_v1_set_app_settings_request_instance.to_dict()
# create an instance of TenantApiTenantV1SetAppSettingsRequest from a dict
tenant_api_tenant_v1_set_app_settings_request_from_dict = TenantApiTenantV1SetAppSettingsRequest.from_dict(tenant_api_tenant_v1_set_app_settings_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


