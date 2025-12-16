# TenantApiTenantV1TenantIdentityProviders


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**identity_provider_id** | [**TenantApiTenantV1IdentityProviderId**](TenantApiTenantV1IdentityProviderId.md) |  | [optional] 
**identity_provider_status** | [**TenantApiTenantV1IdentityProviderStatus**](TenantApiTenantV1IdentityProviderStatus.md) |  | [optional] 
**enforce_mfa** | **str** |  | [optional] 
**enable_mfa** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_tenant_identity_providers import TenantApiTenantV1TenantIdentityProviders

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1TenantIdentityProviders from a JSON string
tenant_api_tenant_v1_tenant_identity_providers_instance = TenantApiTenantV1TenantIdentityProviders.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1TenantIdentityProviders.to_json())

# convert the object into a dict
tenant_api_tenant_v1_tenant_identity_providers_dict = tenant_api_tenant_v1_tenant_identity_providers_instance.to_dict()
# create an instance of TenantApiTenantV1TenantIdentityProviders from a dict
tenant_api_tenant_v1_tenant_identity_providers_from_dict = TenantApiTenantV1TenantIdentityProviders.from_dict(tenant_api_tenant_v1_tenant_identity_providers_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


