# EdfiAdminApiEdfiAdminV1OdsApiConnectionEndpoint


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**access_type_id** | **str** |  | [optional] 
**composites_url** | **str** |  | [optional] 
**resources_url** | **str** |  | [optional] 
**discovery_url** | **str** |  | [optional] 
**discovery_document** | [**EdfiAdminApiEdfiAdminV1OdsApiDiscoveryApi**](EdfiAdminApiEdfiAdminV1OdsApiDiscoveryApi.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ods_api_connection_endpoint import EdfiAdminApiEdfiAdminV1OdsApiConnectionEndpoint

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1OdsApiConnectionEndpoint from a JSON string
edfi_admin_api_edfi_admin_v1_ods_api_connection_endpoint_instance = EdfiAdminApiEdfiAdminV1OdsApiConnectionEndpoint.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1OdsApiConnectionEndpoint.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_ods_api_connection_endpoint_dict = edfi_admin_api_edfi_admin_v1_ods_api_connection_endpoint_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1OdsApiConnectionEndpoint from a dict
edfi_admin_api_edfi_admin_v1_ods_api_connection_endpoint_from_dict = EdfiAdminApiEdfiAdminV1OdsApiConnectionEndpoint.from_dict(edfi_admin_api_edfi_admin_v1_ods_api_connection_endpoint_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


