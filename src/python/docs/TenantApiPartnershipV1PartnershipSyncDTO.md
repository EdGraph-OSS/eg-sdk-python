# TenantApiPartnershipV1PartnershipSyncDTO


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  | [optional] 
**direction** | [**TenantApiPartnershipV1PartnershipSyncDirection**](TenantApiPartnershipV1PartnershipSyncDirection.md) |  | [optional] 
**sync_types** | [**List[TenantApiPartnershipV1PartnershipSyncType]**](TenantApiPartnershipV1PartnershipSyncType.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.tenant_api_partnership_v1_partnership_sync_dto import TenantApiPartnershipV1PartnershipSyncDTO

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiPartnershipV1PartnershipSyncDTO from a JSON string
tenant_api_partnership_v1_partnership_sync_dto_instance = TenantApiPartnershipV1PartnershipSyncDTO.from_json(json)
# print the JSON string representation of the object
print(TenantApiPartnershipV1PartnershipSyncDTO.to_json())

# convert the object into a dict
tenant_api_partnership_v1_partnership_sync_dto_dict = tenant_api_partnership_v1_partnership_sync_dto_instance.to_dict()
# create an instance of TenantApiPartnershipV1PartnershipSyncDTO from a dict
tenant_api_partnership_v1_partnership_sync_dto_from_dict = TenantApiPartnershipV1PartnershipSyncDTO.from_dict(tenant_api_partnership_v1_partnership_sync_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


