# EdfiAdminApiEdfiAdminV1Instance


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Details | [optional] 
**instance_name** | **str** |  | [optional] 
**use_custom_id** | **bool** |  | [optional] 
**custom_id** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**connection_name** | **str** |  | [optional] 
**selected_connection_id** | **str** | Connection | [optional] 
**selected_connection** | [**EdfiAdminApiEdfiAdminV1EdFiConnection**](EdfiAdminApiEdfiAdminV1EdFiConnection.md) |  | [optional] 
**databases** | [**EdfiAdminApiEdfiAdminV1InstanceDatabases**](EdfiAdminApiEdfiAdminV1InstanceDatabases.md) |  | [optional] 
**password** | **str** | API Client | [optional] 
**api_client_key** | **str** |  | [optional] 
**api_client_secret** | **str** |  | [optional] 
**is_api_client_secret_secured** | **str** |  | [optional] 
**tenant_id** | **str** | Metadata | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**api_auth_url** | **str** | URLs | [optional] 
**api_resources_urls** | **List[str]** |  | [optional] [readonly] 
**api_composites_urls** | **List[str]** |  | [optional] [readonly] 
**selected_connection_type** | **str** | Connection | [optional] 
**is_default** | **bool** | IsDefault | [optional] 
**provider** | **str** | Provider | [optional] 
**onboarding** | [**EdfiAdminApiEdfiAdminV1Onboarding**](EdfiAdminApiEdfiAdminV1Onboarding.md) |  | [optional] 
**applications** | [**List[EdfiAdminApiEdfiAdminV1InstanceApplicationProfileResponse]**](EdfiAdminApiEdfiAdminV1InstanceApplicationProfileResponse.md) | Applications | [optional] [readonly] 
**related_instances** | [**List[EdfiAdminApiEdfiAdminV1RelatedInstance]**](EdfiAdminApiEdfiAdminV1RelatedInstance.md) |  | [optional] [readonly] 
**enable_admin_api** | **bool** | Enable Admin API | [optional] 
**state** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_instance import EdfiAdminApiEdfiAdminV1Instance

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1Instance from a JSON string
edfi_admin_api_edfi_admin_v1_instance_instance = EdfiAdminApiEdfiAdminV1Instance.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1Instance.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_instance_dict = edfi_admin_api_edfi_admin_v1_instance_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1Instance from a dict
edfi_admin_api_edfi_admin_v1_instance_from_dict = EdfiAdminApiEdfiAdminV1Instance.from_dict(edfi_admin_api_edfi_admin_v1_instance_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


