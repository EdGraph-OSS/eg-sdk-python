# EdfiAdminApiEdfiAdminV1UpdateInstanceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | The Instance ID or Custom ID | [optional] 
**instance_name** | **str** | Details | [optional] 
**description** | **str** |  | [optional] 
**tenant_id** | **str** | Metadata | [optional] 
**provider** | **str** |  | [optional] 
**state** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_instance_request import EdfiAdminApiEdfiAdminV1UpdateInstanceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1UpdateInstanceRequest from a JSON string
edfi_admin_api_edfi_admin_v1_update_instance_request_instance = EdfiAdminApiEdfiAdminV1UpdateInstanceRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1UpdateInstanceRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_update_instance_request_dict = edfi_admin_api_edfi_admin_v1_update_instance_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1UpdateInstanceRequest from a dict
edfi_admin_api_edfi_admin_v1_update_instance_request_from_dict = EdfiAdminApiEdfiAdminV1UpdateInstanceRequest.from_dict(edfi_admin_api_edfi_admin_v1_update_instance_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


