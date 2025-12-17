# EdfiAdminApiEdfiAdminV1TierOdsApiConnectionListModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**client_id** | **str** |  | [optional] 
**token_url** | **str** |  | [optional] 
**endpoints** | [**List[EdfiAdminApiEdfiAdminV1OdsApiConnectionEndpoint]**](EdfiAdminApiEdfiAdminV1OdsApiConnectionEndpoint.md) |  | [optional] [readonly] 
**metadata_url** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_tier_ods_api_connection_list_model import EdfiAdminApiEdfiAdminV1TierOdsApiConnectionListModel

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1TierOdsApiConnectionListModel from a JSON string
edfi_admin_api_edfi_admin_v1_tier_ods_api_connection_list_model_instance = EdfiAdminApiEdfiAdminV1TierOdsApiConnectionListModel.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1TierOdsApiConnectionListModel.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_tier_ods_api_connection_list_model_dict = edfi_admin_api_edfi_admin_v1_tier_ods_api_connection_list_model_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1TierOdsApiConnectionListModel from a dict
edfi_admin_api_edfi_admin_v1_tier_ods_api_connection_list_model_from_dict = EdfiAdminApiEdfiAdminV1TierOdsApiConnectionListModel.from_dict(edfi_admin_api_edfi_admin_v1_tier_ods_api_connection_list_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


