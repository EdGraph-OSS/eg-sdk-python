# TenantApiTenantV1Organization


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**identifier_type** | **str** |  | [optional] 
**identifier_value** | **str** |  | [optional] 
**discriminator** | **str** |  | [optional] 
**source** | **str** |  | [optional] 
**short_name_of_institution** | **str** |  | [optional] 
**name_of_institution** | **str** |  | [optional] 
**include_in_jwt** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_organization import TenantApiTenantV1Organization

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1Organization from a JSON string
tenant_api_tenant_v1_organization_instance = TenantApiTenantV1Organization.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1Organization.to_json())

# convert the object into a dict
tenant_api_tenant_v1_organization_dict = tenant_api_tenant_v1_organization_instance.to_dict()
# create an instance of TenantApiTenantV1Organization from a dict
tenant_api_tenant_v1_organization_from_dict = TenantApiTenantV1Organization.from_dict(tenant_api_tenant_v1_organization_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


