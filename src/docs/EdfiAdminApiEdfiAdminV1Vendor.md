# EdfiAdminApiEdfiAdminV1Vendor

Common Objects

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**vendor_id** | **int** |  | [optional] 
**vendor_name** | **str** |  | [optional] 
**applications** | **List[int]** | TODO: Changed from application object to applicationId&#39;s to remove cyclic structure | [optional] [readonly] 
**namespace_prefixes** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_vendor import EdfiAdminApiEdfiAdminV1Vendor

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1Vendor from a JSON string
edfi_admin_api_edfi_admin_v1_vendor_instance = EdfiAdminApiEdfiAdminV1Vendor.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1Vendor.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_vendor_dict = edfi_admin_api_edfi_admin_v1_vendor_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1Vendor from a dict
edfi_admin_api_edfi_admin_v1_vendor_from_dict = EdfiAdminApiEdfiAdminV1Vendor.from_dict(edfi_admin_api_edfi_admin_v1_vendor_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


