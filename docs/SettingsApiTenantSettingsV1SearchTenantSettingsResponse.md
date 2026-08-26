# SettingsApiTenantSettingsV1SearchTenantSettingsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[SettingsApiTenantSettingsV1TenantSettingMessage]**](SettingsApiTenantSettingsV1TenantSettingMessage.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.settings_api_tenant_settings_v1_search_tenant_settings_response import SettingsApiTenantSettingsV1SearchTenantSettingsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SettingsApiTenantSettingsV1SearchTenantSettingsResponse from a JSON string
settings_api_tenant_settings_v1_search_tenant_settings_response_instance = SettingsApiTenantSettingsV1SearchTenantSettingsResponse.from_json(json)
# print the JSON string representation of the object
print(SettingsApiTenantSettingsV1SearchTenantSettingsResponse.to_json())

# convert the object into a dict
settings_api_tenant_settings_v1_search_tenant_settings_response_dict = settings_api_tenant_settings_v1_search_tenant_settings_response_instance.to_dict()
# create an instance of SettingsApiTenantSettingsV1SearchTenantSettingsResponse from a dict
settings_api_tenant_settings_v1_search_tenant_settings_response_from_dict = SettingsApiTenantSettingsV1SearchTenantSettingsResponse.from_dict(settings_api_tenant_settings_v1_search_tenant_settings_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


