# TenantApiTenantV1SetAppSettingsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**code** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_set_app_settings_response import TenantApiTenantV1SetAppSettingsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1SetAppSettingsResponse from a JSON string
tenant_api_tenant_v1_set_app_settings_response_instance = TenantApiTenantV1SetAppSettingsResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1SetAppSettingsResponse.to_json())

# convert the object into a dict
tenant_api_tenant_v1_set_app_settings_response_dict = tenant_api_tenant_v1_set_app_settings_response_instance.to_dict()
# create an instance of TenantApiTenantV1SetAppSettingsResponse from a dict
tenant_api_tenant_v1_set_app_settings_response_from_dict = TenantApiTenantV1SetAppSettingsResponse.from_dict(tenant_api_tenant_v1_set_app_settings_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


