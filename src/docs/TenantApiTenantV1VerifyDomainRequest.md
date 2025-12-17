# TenantApiTenantV1VerifyDomainRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**domain_name** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_verify_domain_request import TenantApiTenantV1VerifyDomainRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1VerifyDomainRequest from a JSON string
tenant_api_tenant_v1_verify_domain_request_instance = TenantApiTenantV1VerifyDomainRequest.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1VerifyDomainRequest.to_json())

# convert the object into a dict
tenant_api_tenant_v1_verify_domain_request_dict = tenant_api_tenant_v1_verify_domain_request_instance.to_dict()
# create an instance of TenantApiTenantV1VerifyDomainRequest from a dict
tenant_api_tenant_v1_verify_domain_request_from_dict = TenantApiTenantV1VerifyDomainRequest.from_dict(tenant_api_tenant_v1_verify_domain_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


