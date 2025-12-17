# EdfiAdminApiEdfiAdminV1CloneInstanceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**source_instance_id** | **str** |  | [optional] 
**clone_instance_name** | **str** |  | [optional] 
**clone_instance_use_custom_id** | **bool** |  | [optional] 
**clone_instance_custom_id** | **str** |  | [optional] 
**clone_instance_description** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_clone_instance_request import EdfiAdminApiEdfiAdminV1CloneInstanceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1CloneInstanceRequest from a JSON string
edfi_admin_api_edfi_admin_v1_clone_instance_request_instance = EdfiAdminApiEdfiAdminV1CloneInstanceRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1CloneInstanceRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_clone_instance_request_dict = edfi_admin_api_edfi_admin_v1_clone_instance_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1CloneInstanceRequest from a dict
edfi_admin_api_edfi_admin_v1_clone_instance_request_from_dict = EdfiAdminApiEdfiAdminV1CloneInstanceRequest.from_dict(edfi_admin_api_edfi_admin_v1_clone_instance_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


