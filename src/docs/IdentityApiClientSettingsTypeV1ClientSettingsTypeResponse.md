# IdentityApiClientSettingsTypeV1ClientSettingsTypeResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**code** | **str** |  | [optional] 
**data_type** | **str** |  | [optional] 
**order** | **int** |  | [optional] 
**hidden** | **bool** |  | [optional] 
**html_element** | **str** | Html attributes | [optional] 
**label** | **str** |  | [optional] 
**input_type** | **str** |  | [optional] 
**default_value** | **str** |  | [optional] 
**min_value** | **int** |  | [optional] 
**max_value** | **int** |  | [optional] 
**max_length** | **int** |  | [optional] 
**options** | **List[str]** |  | [optional] [readonly] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_client_settings_type_v1_client_settings_type_response import IdentityApiClientSettingsTypeV1ClientSettingsTypeResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiClientSettingsTypeV1ClientSettingsTypeResponse from a JSON string
identity_api_client_settings_type_v1_client_settings_type_response_instance = IdentityApiClientSettingsTypeV1ClientSettingsTypeResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiClientSettingsTypeV1ClientSettingsTypeResponse.to_json())

# convert the object into a dict
identity_api_client_settings_type_v1_client_settings_type_response_dict = identity_api_client_settings_type_v1_client_settings_type_response_instance.to_dict()
# create an instance of IdentityApiClientSettingsTypeV1ClientSettingsTypeResponse from a dict
identity_api_client_settings_type_v1_client_settings_type_response_from_dict = IdentityApiClientSettingsTypeV1ClientSettingsTypeResponse.from_dict(identity_api_client_settings_type_v1_client_settings_type_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


