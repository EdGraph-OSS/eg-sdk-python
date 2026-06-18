# EdfiAdminApiEdfiAdminV1EdFiConnectionTierListModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tier_id** | **str** |  | [optional] 
**tier_name** | **str** |  | [optional] 
**ods_api_connection** | [**EdfiAdminApiEdfiAdminV1TierOdsApiConnectionListModel**](EdfiAdminApiEdfiAdminV1TierOdsApiConnectionListModel.md) |  | [optional] 
**admin_api_url** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ed_fi_connection_tier_list_model import EdfiAdminApiEdfiAdminV1EdFiConnectionTierListModel

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1EdFiConnectionTierListModel from a JSON string
edfi_admin_api_edfi_admin_v1_ed_fi_connection_tier_list_model_instance = EdfiAdminApiEdfiAdminV1EdFiConnectionTierListModel.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1EdFiConnectionTierListModel.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_ed_fi_connection_tier_list_model_dict = edfi_admin_api_edfi_admin_v1_ed_fi_connection_tier_list_model_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1EdFiConnectionTierListModel from a dict
edfi_admin_api_edfi_admin_v1_ed_fi_connection_tier_list_model_from_dict = EdfiAdminApiEdfiAdminV1EdFiConnectionTierListModel.from_dict(edfi_admin_api_edfi_admin_v1_ed_fi_connection_tier_list_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


