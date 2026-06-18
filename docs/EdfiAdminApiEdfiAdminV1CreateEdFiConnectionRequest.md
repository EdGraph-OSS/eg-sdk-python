# EdfiAdminApiEdfiAdminV1CreateEdFiConnectionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**connection_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**connection_type** | **str** |  | [optional] 
**connection_name** | **str** |  | [optional] 
**ed_fi_version** | **str** |  | [optional] 
**ed_fi_extension** | **str** |  | [optional] 
**metadata_url** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**client_secret** | **str** |  | [optional] 
**token_url** | **str** |  | [optional] 
**resources_url** | **str** |  | [optional] 
**instance_type** | [**EdfiAdminApiEdfiAdminV1InstanceType**](EdfiAdminApiEdfiAdminV1InstanceType.md) |  | [optional] 
**discovery_url** | **str** |  | [optional] 
**metadata_json** | **str** |  | [optional] 
**discovery_document** | [**EdfiAdminApiEdfiAdminV1OdsApiDiscoveryApi**](EdfiAdminApiEdfiAdminV1OdsApiDiscoveryApi.md) |  | [optional] 
**admin_api_url** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_ed_fi_connection_request import EdfiAdminApiEdfiAdminV1CreateEdFiConnectionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1CreateEdFiConnectionRequest from a JSON string
edfi_admin_api_edfi_admin_v1_create_ed_fi_connection_request_instance = EdfiAdminApiEdfiAdminV1CreateEdFiConnectionRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1CreateEdFiConnectionRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_create_ed_fi_connection_request_dict = edfi_admin_api_edfi_admin_v1_create_ed_fi_connection_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1CreateEdFiConnectionRequest from a dict
edfi_admin_api_edfi_admin_v1_create_ed_fi_connection_request_from_dict = EdfiAdminApiEdfiAdminV1CreateEdFiConnectionRequest.from_dict(edfi_admin_api_edfi_admin_v1_create_ed_fi_connection_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


