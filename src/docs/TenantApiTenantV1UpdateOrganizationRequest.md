# TenantApiTenantV1UpdateOrganizationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**identifier_value** | **str** |  | [optional] 
**discriminator** | **str** |  | [optional] 
**source** | **str** |  | [optional] 
**short_name_of_institution** | **str** |  | [optional] 
**name_of_institution** | **str** |  | [optional] 
**include_in_jwt** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_update_organization_request import TenantApiTenantV1UpdateOrganizationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1UpdateOrganizationRequest from a JSON string
tenant_api_tenant_v1_update_organization_request_instance = TenantApiTenantV1UpdateOrganizationRequest.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1UpdateOrganizationRequest.to_json())

# convert the object into a dict
tenant_api_tenant_v1_update_organization_request_dict = tenant_api_tenant_v1_update_organization_request_instance.to_dict()
# create an instance of TenantApiTenantV1UpdateOrganizationRequest from a dict
tenant_api_tenant_v1_update_organization_request_from_dict = TenantApiTenantV1UpdateOrganizationRequest.from_dict(tenant_api_tenant_v1_update_organization_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


