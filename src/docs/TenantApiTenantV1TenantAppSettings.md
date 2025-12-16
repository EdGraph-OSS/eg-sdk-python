# TenantApiTenantV1TenantAppSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**client_id** | **str** |  | [optional] 
**code** | **str** |  | [optional] 
**data** | **str** |  | [optional] 
**data_type** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_tenant_app_settings import TenantApiTenantV1TenantAppSettings

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1TenantAppSettings from a JSON string
tenant_api_tenant_v1_tenant_app_settings_instance = TenantApiTenantV1TenantAppSettings.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1TenantAppSettings.to_json())

# convert the object into a dict
tenant_api_tenant_v1_tenant_app_settings_dict = tenant_api_tenant_v1_tenant_app_settings_instance.to_dict()
# create an instance of TenantApiTenantV1TenantAppSettings from a dict
tenant_api_tenant_v1_tenant_app_settings_from_dict = TenantApiTenantV1TenantAppSettings.from_dict(tenant_api_tenant_v1_tenant_app_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


