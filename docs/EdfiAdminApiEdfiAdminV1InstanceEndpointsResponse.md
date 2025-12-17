# EdfiAdminApiEdfiAdminV1InstanceEndpointsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**auth_url** | **str** |  | [optional] 
**resources_urls** | [**List[EdfiAdminApiEdfiAdminV1ApplicationEndpoint]**](EdfiAdminApiEdfiAdminV1ApplicationEndpoint.md) |  | [optional] [readonly] 
**composites_urls** | [**List[EdfiAdminApiEdfiAdminV1ApplicationEndpoint]**](EdfiAdminApiEdfiAdminV1ApplicationEndpoint.md) |  | [optional] [readonly] 
**discovery_urls** | [**List[EdfiAdminApiEdfiAdminV1ApplicationEndpoint]**](EdfiAdminApiEdfiAdminV1ApplicationEndpoint.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_endpoints_response import EdfiAdminApiEdfiAdminV1InstanceEndpointsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1InstanceEndpointsResponse from a JSON string
edfi_admin_api_edfi_admin_v1_instance_endpoints_response_instance = EdfiAdminApiEdfiAdminV1InstanceEndpointsResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1InstanceEndpointsResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_instance_endpoints_response_dict = edfi_admin_api_edfi_admin_v1_instance_endpoints_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1InstanceEndpointsResponse from a dict
edfi_admin_api_edfi_admin_v1_instance_endpoints_response_from_dict = EdfiAdminApiEdfiAdminV1InstanceEndpointsResponse.from_dict(edfi_admin_api_edfi_admin_v1_instance_endpoints_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


