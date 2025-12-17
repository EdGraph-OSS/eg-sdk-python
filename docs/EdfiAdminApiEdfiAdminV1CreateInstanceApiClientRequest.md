# EdfiAdminApiEdfiAdminV1CreateInstanceApiClientRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**instance_application_id** | **str** |  | [optional] 
**key** | **str** |  | [optional] 
**secret** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_instance_api_client_request import EdfiAdminApiEdfiAdminV1CreateInstanceApiClientRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1CreateInstanceApiClientRequest from a JSON string
edfi_admin_api_edfi_admin_v1_create_instance_api_client_request_instance = EdfiAdminApiEdfiAdminV1CreateInstanceApiClientRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1CreateInstanceApiClientRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_create_instance_api_client_request_dict = edfi_admin_api_edfi_admin_v1_create_instance_api_client_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1CreateInstanceApiClientRequest from a dict
edfi_admin_api_edfi_admin_v1_create_instance_api_client_request_from_dict = EdfiAdminApiEdfiAdminV1CreateInstanceApiClientRequest.from_dict(edfi_admin_api_edfi_admin_v1_create_instance_api_client_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


