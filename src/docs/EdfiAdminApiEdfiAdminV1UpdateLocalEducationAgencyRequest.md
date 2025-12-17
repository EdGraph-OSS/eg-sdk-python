# EdfiAdminApiEdfiAdminV1UpdateLocalEducationAgencyRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**year** | **int** |  | [optional] 
**local_education_agency** | [**EdfiAdminApiEdfiAdminV1LocalEducationAgency**](EdfiAdminApiEdfiAdminV1LocalEducationAgency.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_update_local_education_agency_request import EdfiAdminApiEdfiAdminV1UpdateLocalEducationAgencyRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1UpdateLocalEducationAgencyRequest from a JSON string
edfi_admin_api_edfi_admin_v1_update_local_education_agency_request_instance = EdfiAdminApiEdfiAdminV1UpdateLocalEducationAgencyRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1UpdateLocalEducationAgencyRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_update_local_education_agency_request_dict = edfi_admin_api_edfi_admin_v1_update_local_education_agency_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1UpdateLocalEducationAgencyRequest from a dict
edfi_admin_api_edfi_admin_v1_update_local_education_agency_request_from_dict = EdfiAdminApiEdfiAdminV1UpdateLocalEducationAgencyRequest.from_dict(edfi_admin_api_edfi_admin_v1_update_local_education_agency_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


