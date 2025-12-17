# EdfiAdminApiEdfiAdminV1SetInstanceIsDefaultRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**is_default** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_set_instance_is_default_request import EdfiAdminApiEdfiAdminV1SetInstanceIsDefaultRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1SetInstanceIsDefaultRequest from a JSON string
edfi_admin_api_edfi_admin_v1_set_instance_is_default_request_instance = EdfiAdminApiEdfiAdminV1SetInstanceIsDefaultRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1SetInstanceIsDefaultRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_set_instance_is_default_request_dict = edfi_admin_api_edfi_admin_v1_set_instance_is_default_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1SetInstanceIsDefaultRequest from a dict
edfi_admin_api_edfi_admin_v1_set_instance_is_default_request_from_dict = EdfiAdminApiEdfiAdminV1SetInstanceIsDefaultRequest.from_dict(edfi_admin_api_edfi_admin_v1_set_instance_is_default_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


