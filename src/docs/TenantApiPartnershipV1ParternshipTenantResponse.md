# TenantApiPartnershipV1ParternshipTenantResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**tenant_types** | [**List[TenantApiPartnershipV1TenantType]**](TenantApiPartnershipV1TenantType.md) |  | [optional] [readonly] 
**organization_identifier** | **str** |  | [optional] 
**organization_name** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_partnership_v1_parternship_tenant_response import TenantApiPartnershipV1ParternshipTenantResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiPartnershipV1ParternshipTenantResponse from a JSON string
tenant_api_partnership_v1_parternship_tenant_response_instance = TenantApiPartnershipV1ParternshipTenantResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiPartnershipV1ParternshipTenantResponse.to_json())

# convert the object into a dict
tenant_api_partnership_v1_parternship_tenant_response_dict = tenant_api_partnership_v1_parternship_tenant_response_instance.to_dict()
# create an instance of TenantApiPartnershipV1ParternshipTenantResponse from a dict
tenant_api_partnership_v1_parternship_tenant_response_from_dict = TenantApiPartnershipV1ParternshipTenantResponse.from_dict(tenant_api_partnership_v1_parternship_tenant_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


