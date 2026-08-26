# SettingsApiUserSettingsV1SearchUserSettingsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[SettingsApiUserSettingsV1UserSettingMessage]**](SettingsApiUserSettingsV1UserSettingMessage.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.settings_api_user_settings_v1_search_user_settings_response import SettingsApiUserSettingsV1SearchUserSettingsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SettingsApiUserSettingsV1SearchUserSettingsResponse from a JSON string
settings_api_user_settings_v1_search_user_settings_response_instance = SettingsApiUserSettingsV1SearchUserSettingsResponse.from_json(json)
# print the JSON string representation of the object
print(SettingsApiUserSettingsV1SearchUserSettingsResponse.to_json())

# convert the object into a dict
settings_api_user_settings_v1_search_user_settings_response_dict = settings_api_user_settings_v1_search_user_settings_response_instance.to_dict()
# create an instance of SettingsApiUserSettingsV1SearchUserSettingsResponse from a dict
settings_api_user_settings_v1_search_user_settings_response_from_dict = SettingsApiUserSettingsV1SearchUserSettingsResponse.from_dict(settings_api_user_settings_v1_search_user_settings_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


