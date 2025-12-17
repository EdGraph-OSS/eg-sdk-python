# EdfiAdminApiEdfiAdminV1InstanceResourcesCountListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**year** | **int** |  | [optional] 
**instance_application_id** | **int** |  | [optional] 
**api_client_id** | **int** |  | [optional] 
**resource_name** | **str** |  | [optional] 
**resource_count** | **str** |  | [optional] 
**resource_dependency_order** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_resources_count_list_response import EdfiAdminApiEdfiAdminV1InstanceResourcesCountListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1InstanceResourcesCountListResponse from a JSON string
edfi_admin_api_edfi_admin_v1_instance_resources_count_list_response_instance = EdfiAdminApiEdfiAdminV1InstanceResourcesCountListResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1InstanceResourcesCountListResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_instance_resources_count_list_response_dict = edfi_admin_api_edfi_admin_v1_instance_resources_count_list_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1InstanceResourcesCountListResponse from a dict
edfi_admin_api_edfi_admin_v1_instance_resources_count_list_response_from_dict = EdfiAdminApiEdfiAdminV1InstanceResourcesCountListResponse.from_dict(edfi_admin_api_edfi_admin_v1_instance_resources_count_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


