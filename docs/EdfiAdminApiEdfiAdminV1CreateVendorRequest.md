# EdfiAdminApiEdfiAdminV1CreateVendorRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**vendor_id** | **int** |  | [optional] 
**vendor_name** | **str** |  | [optional] 
**applications** | [**List[EdfiAdminApiEdfiAdminV1EdFiApplication]**](EdfiAdminApiEdfiAdminV1EdFiApplication.md) |  | [optional] [readonly] 
**namespace_prefixes** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_vendor_request import EdfiAdminApiEdfiAdminV1CreateVendorRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1CreateVendorRequest from a JSON string
edfi_admin_api_edfi_admin_v1_create_vendor_request_instance = EdfiAdminApiEdfiAdminV1CreateVendorRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1CreateVendorRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_create_vendor_request_dict = edfi_admin_api_edfi_admin_v1_create_vendor_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1CreateVendorRequest from a dict
edfi_admin_api_edfi_admin_v1_create_vendor_request_from_dict = EdfiAdminApiEdfiAdminV1CreateVendorRequest.from_dict(edfi_admin_api_edfi_admin_v1_create_vendor_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


