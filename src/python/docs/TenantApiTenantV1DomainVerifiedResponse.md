# TenantApiTenantV1DomainVerifiedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**domain_name** | **str** |  | [optional] 
**domain_status** | [**TenantApiTenantV1DomainStatus**](TenantApiTenantV1DomainStatus.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_domain_verified_response import TenantApiTenantV1DomainVerifiedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1DomainVerifiedResponse from a JSON string
tenant_api_tenant_v1_domain_verified_response_instance = TenantApiTenantV1DomainVerifiedResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1DomainVerifiedResponse.to_json())

# convert the object into a dict
tenant_api_tenant_v1_domain_verified_response_dict = tenant_api_tenant_v1_domain_verified_response_instance.to_dict()
# create an instance of TenantApiTenantV1DomainVerifiedResponse from a dict
tenant_api_tenant_v1_domain_verified_response_from_dict = TenantApiTenantV1DomainVerifiedResponse.from_dict(tenant_api_tenant_v1_domain_verified_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


