# TenantApiTenantV1UpdateDomainRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**old_domain_name** | **str** |  | [optional] 
**new_domain_name** | **str** |  | [optional] 
**domain_status** | [**TenantApiTenantV1DomainStatus**](TenantApiTenantV1DomainStatus.md) |  | [optional] 
**auto_assign_users** | **bool** |  | [optional] 
**manually_verified** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_update_domain_request import TenantApiTenantV1UpdateDomainRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1UpdateDomainRequest from a JSON string
tenant_api_tenant_v1_update_domain_request_instance = TenantApiTenantV1UpdateDomainRequest.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1UpdateDomainRequest.to_json())

# convert the object into a dict
tenant_api_tenant_v1_update_domain_request_dict = tenant_api_tenant_v1_update_domain_request_instance.to_dict()
# create an instance of TenantApiTenantV1UpdateDomainRequest from a dict
tenant_api_tenant_v1_update_domain_request_from_dict = TenantApiTenantV1UpdateDomainRequest.from_dict(tenant_api_tenant_v1_update_domain_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


