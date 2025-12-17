# IMSAdminApiV1ConnectionsConnectionProfileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**connection_id** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**allowed_tenants** | **List[str]** |  | [optional] [readonly] 
**name** | **str** |  | [optional] 
**details** | [**List[IMSAdminApiV1ConnectionsConnectionDetails]**](IMSAdminApiV1ConnectionsConnectionDetails.md) |  | [optional] [readonly] 
**tiers** | [**List[IMSAdminApiV1TiersTier]**](IMSAdminApiV1TiersTier.md) |  | [optional] [readonly] 
**backup_codes** | [**List[IMSAdminApiV1DbBackupCodesDbBackupCode]**](IMSAdminApiV1DbBackupCodesDbBackupCode.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ims_admin_api_v1_connections_connection_profile_response import IMSAdminApiV1ConnectionsConnectionProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IMSAdminApiV1ConnectionsConnectionProfileResponse from a JSON string
ims_admin_api_v1_connections_connection_profile_response_instance = IMSAdminApiV1ConnectionsConnectionProfileResponse.from_json(json)
# print the JSON string representation of the object
print(IMSAdminApiV1ConnectionsConnectionProfileResponse.to_json())

# convert the object into a dict
ims_admin_api_v1_connections_connection_profile_response_dict = ims_admin_api_v1_connections_connection_profile_response_instance.to_dict()
# create an instance of IMSAdminApiV1ConnectionsConnectionProfileResponse from a dict
ims_admin_api_v1_connections_connection_profile_response_from_dict = IMSAdminApiV1ConnectionsConnectionProfileResponse.from_dict(ims_admin_api_v1_connections_connection_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


