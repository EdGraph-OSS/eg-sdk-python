# TenantApiPartnershipV1PartnershipResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**partner_tenant** | [**TenantApiPartnershipV1ParternshipTenantResponse**](TenantApiPartnershipV1ParternshipTenantResponse.md) |  | [optional] 
**partnership_type** | **str** |  | [optional] 
**related_tenants** | [**List[TenantApiPartnershipV1ParternshipTenantResponse]**](TenantApiPartnershipV1ParternshipTenantResponse.md) |  | [optional] [readonly] 
**partnership_sync** | [**TenantApiPartnershipV1PartnershipSyncDTO**](TenantApiPartnershipV1PartnershipSyncDTO.md) |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_partnership_v1_partnership_response import TenantApiPartnershipV1PartnershipResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiPartnershipV1PartnershipResponse from a JSON string
tenant_api_partnership_v1_partnership_response_instance = TenantApiPartnershipV1PartnershipResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiPartnershipV1PartnershipResponse.to_json())

# convert the object into a dict
tenant_api_partnership_v1_partnership_response_dict = tenant_api_partnership_v1_partnership_response_instance.to_dict()
# create an instance of TenantApiPartnershipV1PartnershipResponse from a dict
tenant_api_partnership_v1_partnership_response_from_dict = TenantApiPartnershipV1PartnershipResponse.from_dict(tenant_api_partnership_v1_partnership_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


