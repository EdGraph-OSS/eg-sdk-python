# TenantApiTenantV1CreateDomainRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**domain_name** | **str** |  | [optional] 
**domain_status** | [**TenantApiTenantV1DomainStatus**](TenantApiTenantV1DomainStatus.md) |  | [optional] 
**auto_assign_users** | **bool** |  | [optional] 
**manually_verified** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_create_domain_request import TenantApiTenantV1CreateDomainRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1CreateDomainRequest from a JSON string
tenant_api_tenant_v1_create_domain_request_instance = TenantApiTenantV1CreateDomainRequest.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1CreateDomainRequest.to_json())

# convert the object into a dict
tenant_api_tenant_v1_create_domain_request_dict = tenant_api_tenant_v1_create_domain_request_instance.to_dict()
# create an instance of TenantApiTenantV1CreateDomainRequest from a dict
tenant_api_tenant_v1_create_domain_request_from_dict = TenantApiTenantV1CreateDomainRequest.from_dict(tenant_api_tenant_v1_create_domain_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


