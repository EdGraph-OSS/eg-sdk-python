# EdfiAdminApiEdfiAdminV1UpdateSpecificationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**specification** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_specification_request import EdfiAdminApiEdfiAdminV1UpdateSpecificationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1UpdateSpecificationRequest from a JSON string
edfi_admin_api_edfi_admin_v1_update_specification_request_instance = EdfiAdminApiEdfiAdminV1UpdateSpecificationRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1UpdateSpecificationRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_update_specification_request_dict = edfi_admin_api_edfi_admin_v1_update_specification_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1UpdateSpecificationRequest from a dict
edfi_admin_api_edfi_admin_v1_update_specification_request_from_dict = EdfiAdminApiEdfiAdminV1UpdateSpecificationRequest.from_dict(edfi_admin_api_edfi_admin_v1_update_specification_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


