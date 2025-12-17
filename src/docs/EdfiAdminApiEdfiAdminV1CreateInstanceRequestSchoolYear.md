# EdfiAdminApiEdfiAdminV1CreateInstanceRequestSchoolYear


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**year** | **int** |  | [optional] 
**selected_tier_id** | **str** |  | [optional] 
**ods_backup_code** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_instance_request_school_year import EdfiAdminApiEdfiAdminV1CreateInstanceRequestSchoolYear

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1CreateInstanceRequestSchoolYear from a JSON string
edfi_admin_api_edfi_admin_v1_create_instance_request_school_year_instance = EdfiAdminApiEdfiAdminV1CreateInstanceRequestSchoolYear.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1CreateInstanceRequestSchoolYear.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_create_instance_request_school_year_dict = edfi_admin_api_edfi_admin_v1_create_instance_request_school_year_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1CreateInstanceRequestSchoolYear from a dict
edfi_admin_api_edfi_admin_v1_create_instance_request_school_year_from_dict = EdfiAdminApiEdfiAdminV1CreateInstanceRequestSchoolYear.from_dict(edfi_admin_api_edfi_admin_v1_create_instance_request_school_year_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


