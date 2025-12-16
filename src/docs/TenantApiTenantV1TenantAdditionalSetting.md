# TenantApiTenantV1TenantAdditionalSetting


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**show_local_login_option_to_tenant_admins** | **bool** |  | [optional] 
**grace_period_mfa_expiry_date** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_tenant_additional_setting import TenantApiTenantV1TenantAdditionalSetting

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1TenantAdditionalSetting from a JSON string
tenant_api_tenant_v1_tenant_additional_setting_instance = TenantApiTenantV1TenantAdditionalSetting.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1TenantAdditionalSetting.to_json())

# convert the object into a dict
tenant_api_tenant_v1_tenant_additional_setting_dict = tenant_api_tenant_v1_tenant_additional_setting_instance.to_dict()
# create an instance of TenantApiTenantV1TenantAdditionalSetting from a dict
tenant_api_tenant_v1_tenant_additional_setting_from_dict = TenantApiTenantV1TenantAdditionalSetting.from_dict(tenant_api_tenant_v1_tenant_additional_setting_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


