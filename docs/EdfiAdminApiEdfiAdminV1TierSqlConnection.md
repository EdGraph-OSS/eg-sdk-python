# EdfiAdminApiEdfiAdminV1TierSqlConnection


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sql_server** | **str** |  | [optional] 
**sql_server_user_name** | **str** |  | [optional] 
**sql_server_password** | **str** |  | [optional] 
**azure_subscription_id** | **str** |  | [optional] 
**azure_resource_group_name** | **str** |  | [optional] 
**azure_server_name** | **str** |  | [optional] 
**azure_server_elastic_pool_name** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_tier_sql_connection import EdfiAdminApiEdfiAdminV1TierSqlConnection

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1TierSqlConnection from a JSON string
edfi_admin_api_edfi_admin_v1_tier_sql_connection_instance = EdfiAdminApiEdfiAdminV1TierSqlConnection.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1TierSqlConnection.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_tier_sql_connection_dict = edfi_admin_api_edfi_admin_v1_tier_sql_connection_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1TierSqlConnection from a dict
edfi_admin_api_edfi_admin_v1_tier_sql_connection_from_dict = EdfiAdminApiEdfiAdminV1TierSqlConnection.from_dict(edfi_admin_api_edfi_admin_v1_tier_sql_connection_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


