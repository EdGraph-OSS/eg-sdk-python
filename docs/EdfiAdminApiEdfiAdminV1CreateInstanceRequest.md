# EdfiAdminApiEdfiAdminV1CreateInstanceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**instance_name** | **str** | Details | [optional] 
**use_custom_id** | **bool** |  | [optional] 
**custom_id** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**database_engine** | **str** | Connection | [optional] 
**selected_connection_id** | **str** |  | [optional] 
**school_years** | [**List[EdfiAdminApiEdfiAdminV1CreateInstanceRequestSchoolYear]**](EdfiAdminApiEdfiAdminV1CreateInstanceRequestSchoolYear.md) | School Years | [optional] [readonly] 
**tenant_id** | **str** | Metadata | [optional] 
**provider** | **str** | Provider | [optional] 
**enable_admin_api** | **bool** | Enable Admin API | [optional] 
**state** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_instance_request import EdfiAdminApiEdfiAdminV1CreateInstanceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1CreateInstanceRequest from a JSON string
edfi_admin_api_edfi_admin_v1_create_instance_request_instance = EdfiAdminApiEdfiAdminV1CreateInstanceRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1CreateInstanceRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_create_instance_request_dict = edfi_admin_api_edfi_admin_v1_create_instance_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1CreateInstanceRequest from a dict
edfi_admin_api_edfi_admin_v1_create_instance_request_from_dict = EdfiAdminApiEdfiAdminV1CreateInstanceRequest.from_dict(edfi_admin_api_edfi_admin_v1_create_instance_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


