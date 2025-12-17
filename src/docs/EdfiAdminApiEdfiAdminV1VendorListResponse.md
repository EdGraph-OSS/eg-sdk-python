# EdfiAdminApiEdfiAdminV1VendorListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**vendor_id** | **int** |  | [optional] 
**vendor_name** | **str** |  | [optional] 
**namespace_prefixes** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_vendor_list_response import EdfiAdminApiEdfiAdminV1VendorListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1VendorListResponse from a JSON string
edfi_admin_api_edfi_admin_v1_vendor_list_response_instance = EdfiAdminApiEdfiAdminV1VendorListResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1VendorListResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_vendor_list_response_dict = edfi_admin_api_edfi_admin_v1_vendor_list_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1VendorListResponse from a dict
edfi_admin_api_edfi_admin_v1_vendor_list_response_from_dict = EdfiAdminApiEdfiAdminV1VendorListResponse.from_dict(edfi_admin_api_edfi_admin_v1_vendor_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


