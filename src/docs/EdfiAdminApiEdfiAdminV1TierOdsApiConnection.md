# EdfiAdminApiEdfiAdminV1TierOdsApiConnection


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**client_id** | **str** |  | [optional] 
**client_secret** | **str** |  | [optional] 
**token_url** | **str** |  | [optional] 
**endpoints** | [**List[EdfiAdminApiEdfiAdminV1OdsApiConnectionEndpoint]**](EdfiAdminApiEdfiAdminV1OdsApiConnectionEndpoint.md) |  | [optional] [readonly] 
**metadata_url** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_tier_ods_api_connection import EdfiAdminApiEdfiAdminV1TierOdsApiConnection

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1TierOdsApiConnection from a JSON string
edfi_admin_api_edfi_admin_v1_tier_ods_api_connection_instance = EdfiAdminApiEdfiAdminV1TierOdsApiConnection.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1TierOdsApiConnection.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_tier_ods_api_connection_dict = edfi_admin_api_edfi_admin_v1_tier_ods_api_connection_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1TierOdsApiConnection from a dict
edfi_admin_api_edfi_admin_v1_tier_ods_api_connection_from_dict = EdfiAdminApiEdfiAdminV1TierOdsApiConnection.from_dict(edfi_admin_api_edfi_admin_v1_tier_ods_api_connection_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


