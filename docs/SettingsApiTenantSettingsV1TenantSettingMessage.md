# SettingsApiTenantSettingsV1TenantSettingMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**setting_type_id** | **str** |  | [optional] 
**application_id** | **str** |  | [optional] 
**schema_version** | **str** |  | [optional] 
**value** | [**GoogleProtobufWellKnownTypesValue**](GoogleProtobufWellKnownTypesValue.md) |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**provider** | **str** |  | [optional] 
**code** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.settings_api_tenant_settings_v1_tenant_setting_message import SettingsApiTenantSettingsV1TenantSettingMessage

# TODO update the JSON string below
json = "{}"
# create an instance of SettingsApiTenantSettingsV1TenantSettingMessage from a JSON string
settings_api_tenant_settings_v1_tenant_setting_message_instance = SettingsApiTenantSettingsV1TenantSettingMessage.from_json(json)
# print the JSON string representation of the object
print(SettingsApiTenantSettingsV1TenantSettingMessage.to_json())

# convert the object into a dict
settings_api_tenant_settings_v1_tenant_setting_message_dict = settings_api_tenant_settings_v1_tenant_setting_message_instance.to_dict()
# create an instance of SettingsApiTenantSettingsV1TenantSettingMessage from a dict
settings_api_tenant_settings_v1_tenant_setting_message_from_dict = SettingsApiTenantSettingsV1TenantSettingMessage.from_dict(settings_api_tenant_settings_v1_tenant_setting_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


