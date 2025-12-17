# EdfiAdminApiEdfiAdminV1EdFiOdsBackupDescriptorsPaginatedItemsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EdfiAdminApiEdfiAdminV1EdFiOdsBackupDescriptor]**](EdfiAdminApiEdfiAdminV1EdFiOdsBackupDescriptor.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ed_fi_ods_backup_descriptors_paginated_items_response import EdfiAdminApiEdfiAdminV1EdFiOdsBackupDescriptorsPaginatedItemsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1EdFiOdsBackupDescriptorsPaginatedItemsResponse from a JSON string
edfi_admin_api_edfi_admin_v1_ed_fi_ods_backup_descriptors_paginated_items_response_instance = EdfiAdminApiEdfiAdminV1EdFiOdsBackupDescriptorsPaginatedItemsResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1EdFiOdsBackupDescriptorsPaginatedItemsResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_ed_fi_ods_backup_descriptors_paginated_items_response_dict = edfi_admin_api_edfi_admin_v1_ed_fi_ods_backup_descriptors_paginated_items_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1EdFiOdsBackupDescriptorsPaginatedItemsResponse from a dict
edfi_admin_api_edfi_admin_v1_ed_fi_ods_backup_descriptors_paginated_items_response_from_dict = EdfiAdminApiEdfiAdminV1EdFiOdsBackupDescriptorsPaginatedItemsResponse.from_dict(edfi_admin_api_edfi_admin_v1_ed_fi_ods_backup_descriptors_paginated_items_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


