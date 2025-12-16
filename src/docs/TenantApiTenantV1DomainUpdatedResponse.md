# TenantApiTenantV1DomainUpdatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**old_domain_name** | **str** |  | [optional] 
**new_domain_name** | **str** |  | [optional] 
**domain_status** | [**TenantApiTenantV1DomainStatus**](TenantApiTenantV1DomainStatus.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_domain_updated_response import TenantApiTenantV1DomainUpdatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1DomainUpdatedResponse from a JSON string
tenant_api_tenant_v1_domain_updated_response_instance = TenantApiTenantV1DomainUpdatedResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1DomainUpdatedResponse.to_json())

# convert the object into a dict
tenant_api_tenant_v1_domain_updated_response_dict = tenant_api_tenant_v1_domain_updated_response_instance.to_dict()
# create an instance of TenantApiTenantV1DomainUpdatedResponse from a dict
tenant_api_tenant_v1_domain_updated_response_from_dict = TenantApiTenantV1DomainUpdatedResponse.from_dict(tenant_api_tenant_v1_domain_updated_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


