# EdfiAdminApiEdfiAdminV1SpecificationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**specification** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_specification_response import EdfiAdminApiEdfiAdminV1SpecificationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1SpecificationResponse from a JSON string
edfi_admin_api_edfi_admin_v1_specification_response_instance = EdfiAdminApiEdfiAdminV1SpecificationResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1SpecificationResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_specification_response_dict = edfi_admin_api_edfi_admin_v1_specification_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1SpecificationResponse from a dict
edfi_admin_api_edfi_admin_v1_specification_response_from_dict = EdfiAdminApiEdfiAdminV1SpecificationResponse.from_dict(edfi_admin_api_edfi_admin_v1_specification_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


