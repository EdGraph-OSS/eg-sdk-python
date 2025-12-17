# EdfiAdminApiEdfiAdminV1AddRelatedInstancesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**related_instance_ids** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_add_related_instances_request import EdfiAdminApiEdfiAdminV1AddRelatedInstancesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1AddRelatedInstancesRequest from a JSON string
edfi_admin_api_edfi_admin_v1_add_related_instances_request_instance = EdfiAdminApiEdfiAdminV1AddRelatedInstancesRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1AddRelatedInstancesRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_add_related_instances_request_dict = edfi_admin_api_edfi_admin_v1_add_related_instances_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1AddRelatedInstancesRequest from a dict
edfi_admin_api_edfi_admin_v1_add_related_instances_request_from_dict = EdfiAdminApiEdfiAdminV1AddRelatedInstancesRequest.from_dict(edfi_admin_api_edfi_admin_v1_add_related_instances_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


