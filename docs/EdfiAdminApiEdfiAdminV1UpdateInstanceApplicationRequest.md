# EdfiAdminApiEdfiAdminV1UpdateInstanceApplicationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**instance_application_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_instance_application_request import EdfiAdminApiEdfiAdminV1UpdateInstanceApplicationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1UpdateInstanceApplicationRequest from a JSON string
edfi_admin_api_edfi_admin_v1_update_instance_application_request_instance = EdfiAdminApiEdfiAdminV1UpdateInstanceApplicationRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1UpdateInstanceApplicationRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_update_instance_application_request_dict = edfi_admin_api_edfi_admin_v1_update_instance_application_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1UpdateInstanceApplicationRequest from a dict
edfi_admin_api_edfi_admin_v1_update_instance_application_request_from_dict = EdfiAdminApiEdfiAdminV1UpdateInstanceApplicationRequest.from_dict(edfi_admin_api_edfi_admin_v1_update_instance_application_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


