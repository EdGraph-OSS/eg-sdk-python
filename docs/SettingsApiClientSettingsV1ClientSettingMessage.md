# SettingsApiClientSettingsV1ClientSettingMessage


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
from edgraph_platform_client.models.settings_api_client_settings_v1_client_setting_message import SettingsApiClientSettingsV1ClientSettingMessage

# TODO update the JSON string below
json = "{}"
# create an instance of SettingsApiClientSettingsV1ClientSettingMessage from a JSON string
settings_api_client_settings_v1_client_setting_message_instance = SettingsApiClientSettingsV1ClientSettingMessage.from_json(json)
# print the JSON string representation of the object
print(SettingsApiClientSettingsV1ClientSettingMessage.to_json())

# convert the object into a dict
settings_api_client_settings_v1_client_setting_message_dict = settings_api_client_settings_v1_client_setting_message_instance.to_dict()
# create an instance of SettingsApiClientSettingsV1ClientSettingMessage from a dict
settings_api_client_settings_v1_client_setting_message_from_dict = SettingsApiClientSettingsV1ClientSettingMessage.from_dict(settings_api_client_settings_v1_client_setting_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


