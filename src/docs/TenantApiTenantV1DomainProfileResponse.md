# TenantApiTenantV1DomainProfileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**domain_name** | **str** |  | [optional] 
**domain_status** | [**TenantApiTenantV1DomainStatus**](TenantApiTenantV1DomainStatus.md) |  | [optional] 
**auto_assign_users** | **bool** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_domain_profile_response import TenantApiTenantV1DomainProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1DomainProfileResponse from a JSON string
tenant_api_tenant_v1_domain_profile_response_instance = TenantApiTenantV1DomainProfileResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1DomainProfileResponse.to_json())

# convert the object into a dict
tenant_api_tenant_v1_domain_profile_response_dict = tenant_api_tenant_v1_domain_profile_response_instance.to_dict()
# create an instance of TenantApiTenantV1DomainProfileResponse from a dict
tenant_api_tenant_v1_domain_profile_response_from_dict = TenantApiTenantV1DomainProfileResponse.from_dict(tenant_api_tenant_v1_domain_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


