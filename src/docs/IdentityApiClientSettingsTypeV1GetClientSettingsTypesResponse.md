# IdentityApiClientSettingsTypeV1GetClientSettingsTypesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[IdentityApiClientSettingsTypeV1ClientSettingsTypeResponse]**](IdentityApiClientSettingsTypeV1ClientSettingsTypeResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_client_settings_type_v1_get_client_settings_types_response import IdentityApiClientSettingsTypeV1GetClientSettingsTypesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiClientSettingsTypeV1GetClientSettingsTypesResponse from a JSON string
identity_api_client_settings_type_v1_get_client_settings_types_response_instance = IdentityApiClientSettingsTypeV1GetClientSettingsTypesResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiClientSettingsTypeV1GetClientSettingsTypesResponse.to_json())

# convert the object into a dict
identity_api_client_settings_type_v1_get_client_settings_types_response_dict = identity_api_client_settings_type_v1_get_client_settings_types_response_instance.to_dict()
# create an instance of IdentityApiClientSettingsTypeV1GetClientSettingsTypesResponse from a dict
identity_api_client_settings_type_v1_get_client_settings_types_response_from_dict = IdentityApiClientSettingsTypeV1GetClientSettingsTypesResponse.from_dict(identity_api_client_settings_type_v1_get_client_settings_types_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


