# EdfiAdminApiEdfiAdminV1EdFiConnectionTier


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tier_id** | **str** |  | [optional] 
**tier_name** | **str** |  | [optional] 
**ods_api_connection** | [**EdfiAdminApiEdfiAdminV1TierOdsApiConnection**](EdfiAdminApiEdfiAdminV1TierOdsApiConnection.md) |  | [optional] 
**sql_connection** | [**EdfiAdminApiEdfiAdminV1TierSqlConnection**](EdfiAdminApiEdfiAdminV1TierSqlConnection.md) |  | [optional] 
**admin_api_url** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ed_fi_connection_tier import EdfiAdminApiEdfiAdminV1EdFiConnectionTier

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1EdFiConnectionTier from a JSON string
edfi_admin_api_edfi_admin_v1_ed_fi_connection_tier_instance = EdfiAdminApiEdfiAdminV1EdFiConnectionTier.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1EdFiConnectionTier.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_ed_fi_connection_tier_dict = edfi_admin_api_edfi_admin_v1_ed_fi_connection_tier_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1EdFiConnectionTier from a dict
edfi_admin_api_edfi_admin_v1_ed_fi_connection_tier_from_dict = EdfiAdminApiEdfiAdminV1EdFiConnectionTier.from_dict(edfi_admin_api_edfi_admin_v1_ed_fi_connection_tier_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


