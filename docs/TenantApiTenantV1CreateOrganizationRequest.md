# TenantApiTenantV1CreateOrganizationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**identifier_type** | **str** |  | [optional] 
**identifier_value** | **str** |  | [optional] 
**short_name_of_institution** | **str** |  | [optional] 
**name_of_institution** | **str** |  | [optional] 
**discriminator** | **str** |  | [optional] 
**source** | **str** |  | [optional] 
**include_in_jwt** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_create_organization_request import TenantApiTenantV1CreateOrganizationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1CreateOrganizationRequest from a JSON string
tenant_api_tenant_v1_create_organization_request_instance = TenantApiTenantV1CreateOrganizationRequest.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1CreateOrganizationRequest.to_json())

# convert the object into a dict
tenant_api_tenant_v1_create_organization_request_dict = tenant_api_tenant_v1_create_organization_request_instance.to_dict()
# create an instance of TenantApiTenantV1CreateOrganizationRequest from a dict
tenant_api_tenant_v1_create_organization_request_from_dict = TenantApiTenantV1CreateOrganizationRequest.from_dict(tenant_api_tenant_v1_create_organization_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


