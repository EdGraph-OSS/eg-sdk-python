# EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**instance_application_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**api_clients** | [**List[EdfiAdminApiEdfiAdminV1InstanceApiClientListResponse]**](EdfiAdminApiEdfiAdminV1InstanceApiClientListResponse.md) |  | [optional] [readonly] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance_applications_list_response import EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponse from a JSON string
edfi_admin_api_edfi_admin_v1_instance_applications_list_response_instance = EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_instance_applications_list_response_dict = edfi_admin_api_edfi_admin_v1_instance_applications_list_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponse from a dict
edfi_admin_api_edfi_admin_v1_instance_applications_list_response_from_dict = EdfiAdminApiEdfiAdminV1InstanceApplicationsListResponse.from_dict(edfi_admin_api_edfi_admin_v1_instance_applications_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


