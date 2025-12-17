# EdfiAdminApiEdfiAdminV1ChangeDatabaseTierRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**instance_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**year** | **int** |  | [optional] 
**selected_tier** | [**EdfiAdminApiEdfiAdminV1DatabaseTier**](EdfiAdminApiEdfiAdminV1DatabaseTier.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_change_database_tier_request import EdfiAdminApiEdfiAdminV1ChangeDatabaseTierRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1ChangeDatabaseTierRequest from a JSON string
edfi_admin_api_edfi_admin_v1_change_database_tier_request_instance = EdfiAdminApiEdfiAdminV1ChangeDatabaseTierRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1ChangeDatabaseTierRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_change_database_tier_request_dict = edfi_admin_api_edfi_admin_v1_change_database_tier_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1ChangeDatabaseTierRequest from a dict
edfi_admin_api_edfi_admin_v1_change_database_tier_request_from_dict = EdfiAdminApiEdfiAdminV1ChangeDatabaseTierRequest.from_dict(edfi_admin_api_edfi_admin_v1_change_database_tier_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


