# EdfiAdminApiEdfiAdminV1ResourceItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**resource_name** | **str** |  | [optional] 
**var_schema** | **str** |  | [optional] 
**dependencies** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_resource_item import EdfiAdminApiEdfiAdminV1ResourceItem

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1ResourceItem from a JSON string
edfi_admin_api_edfi_admin_v1_resource_item_instance = EdfiAdminApiEdfiAdminV1ResourceItem.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1ResourceItem.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_resource_item_dict = edfi_admin_api_edfi_admin_v1_resource_item_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1ResourceItem from a dict
edfi_admin_api_edfi_admin_v1_resource_item_from_dict = EdfiAdminApiEdfiAdminV1ResourceItem.from_dict(edfi_admin_api_edfi_admin_v1_resource_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


