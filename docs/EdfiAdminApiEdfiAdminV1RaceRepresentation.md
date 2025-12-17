# EdfiAdminApiEdfiAdminV1RaceRepresentation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**value** | **str** |  | [optional] 
**percent_of_total** | **float** |  | [optional] 
**display_name** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_race_representation import EdfiAdminApiEdfiAdminV1RaceRepresentation

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1RaceRepresentation from a JSON string
edfi_admin_api_edfi_admin_v1_race_representation_instance = EdfiAdminApiEdfiAdminV1RaceRepresentation.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1RaceRepresentation.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_race_representation_dict = edfi_admin_api_edfi_admin_v1_race_representation_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1RaceRepresentation from a dict
edfi_admin_api_edfi_admin_v1_race_representation_from_dict = EdfiAdminApiEdfiAdminV1RaceRepresentation.from_dict(edfi_admin_api_edfi_admin_v1_race_representation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


