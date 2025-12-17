# TenantApiTenantV1GetAppSettingsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[TenantApiTenantV1TenantAppSettings]**](TenantApiTenantV1TenantAppSettings.md) |  | [optional] [readonly] 
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_get_app_settings_response import TenantApiTenantV1GetAppSettingsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1GetAppSettingsResponse from a JSON string
tenant_api_tenant_v1_get_app_settings_response_instance = TenantApiTenantV1GetAppSettingsResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1GetAppSettingsResponse.to_json())

# convert the object into a dict
tenant_api_tenant_v1_get_app_settings_response_dict = tenant_api_tenant_v1_get_app_settings_response_instance.to_dict()
# create an instance of TenantApiTenantV1GetAppSettingsResponse from a dict
tenant_api_tenant_v1_get_app_settings_response_from_dict = TenantApiTenantV1GetAppSettingsResponse.from_dict(tenant_api_tenant_v1_get_app_settings_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


