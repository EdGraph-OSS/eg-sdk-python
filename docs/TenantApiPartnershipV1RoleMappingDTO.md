# TenantApiPartnershipV1RoleMappingDTO


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**partner_role** | **str** |  | [optional] 
**granted_role** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_partnership_v1_role_mapping_dto import TenantApiPartnershipV1RoleMappingDTO

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiPartnershipV1RoleMappingDTO from a JSON string
tenant_api_partnership_v1_role_mapping_dto_instance = TenantApiPartnershipV1RoleMappingDTO.from_json(json)
# print the JSON string representation of the object
print(TenantApiPartnershipV1RoleMappingDTO.to_json())

# convert the object into a dict
tenant_api_partnership_v1_role_mapping_dto_dict = tenant_api_partnership_v1_role_mapping_dto_instance.to_dict()
# create an instance of TenantApiPartnershipV1RoleMappingDTO from a dict
tenant_api_partnership_v1_role_mapping_dto_from_dict = TenantApiPartnershipV1RoleMappingDTO.from_dict(tenant_api_partnership_v1_role_mapping_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


