# TenantApiTenantV1TenantSettingTypesListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**code** | **str** |  | [optional] 
**data_type** | **str** |  | [optional] 
**order** | **int** |  | [optional] 
**hidden** | **bool** |  | [optional] 
**html_element** | **str** |  | [optional] 
**label** | **str** |  | [optional] 
**input_type** | **str** |  | [optional] 
**default_value** | **str** |  | [optional] 
**min_value** | **int** |  | [optional] 
**max_value** | **int** |  | [optional] 
**max_length** | **int** |  | [optional] 
**attributes** | [**List[TenantApiTenantV1TenantSettingsTypeAttribute]**](TenantApiTenantV1TenantSettingsTypeAttribute.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_tenant_setting_types_list_response import TenantApiTenantV1TenantSettingTypesListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1TenantSettingTypesListResponse from a JSON string
tenant_api_tenant_v1_tenant_setting_types_list_response_instance = TenantApiTenantV1TenantSettingTypesListResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1TenantSettingTypesListResponse.to_json())

# convert the object into a dict
tenant_api_tenant_v1_tenant_setting_types_list_response_dict = tenant_api_tenant_v1_tenant_setting_types_list_response_instance.to_dict()
# create an instance of TenantApiTenantV1TenantSettingTypesListResponse from a dict
tenant_api_tenant_v1_tenant_setting_types_list_response_from_dict = TenantApiTenantV1TenantSettingTypesListResponse.from_dict(tenant_api_tenant_v1_tenant_setting_types_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


