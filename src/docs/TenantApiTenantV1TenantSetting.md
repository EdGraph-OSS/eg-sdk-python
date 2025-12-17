# TenantApiTenantV1TenantSetting


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | [optional] 
**value** | **str** |  | [optional] 
**data_type** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_tenant_setting import TenantApiTenantV1TenantSetting

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1TenantSetting from a JSON string
tenant_api_tenant_v1_tenant_setting_instance = TenantApiTenantV1TenantSetting.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1TenantSetting.to_json())

# convert the object into a dict
tenant_api_tenant_v1_tenant_setting_dict = tenant_api_tenant_v1_tenant_setting_instance.to_dict()
# create an instance of TenantApiTenantV1TenantSetting from a dict
tenant_api_tenant_v1_tenant_setting_from_dict = TenantApiTenantV1TenantSetting.from_dict(tenant_api_tenant_v1_tenant_setting_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


