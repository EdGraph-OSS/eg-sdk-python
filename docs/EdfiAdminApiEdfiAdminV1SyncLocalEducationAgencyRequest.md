# EdfiAdminApiEdfiAdminV1SyncLocalEducationAgencyRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**year** | **int** |  | [optional] 
**ed_org_id** | **int** |  | [optional] 
**ed_org_guid** | **str** |  | [optional] 
**entries** | [**List[EdfiAdminApiEdfiAdminV1SyncEntry]**](EdfiAdminApiEdfiAdminV1SyncEntry.md) |  | [optional] [readonly] 
**assign_to_existing_applications** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_sync_local_education_agency_request import EdfiAdminApiEdfiAdminV1SyncLocalEducationAgencyRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1SyncLocalEducationAgencyRequest from a JSON string
edfi_admin_api_edfi_admin_v1_sync_local_education_agency_request_instance = EdfiAdminApiEdfiAdminV1SyncLocalEducationAgencyRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1SyncLocalEducationAgencyRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_sync_local_education_agency_request_dict = edfi_admin_api_edfi_admin_v1_sync_local_education_agency_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1SyncLocalEducationAgencyRequest from a dict
edfi_admin_api_edfi_admin_v1_sync_local_education_agency_request_from_dict = EdfiAdminApiEdfiAdminV1SyncLocalEducationAgencyRequest.from_dict(edfi_admin_api_edfi_admin_v1_sync_local_education_agency_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


