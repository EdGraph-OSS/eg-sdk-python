# EdfiAdminApiEdfiAdminV1LocalEducationAgencyCreatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**local_education_agency** | [**EdfiAdminApiEdfiAdminV1LocalEducationAgency**](EdfiAdminApiEdfiAdminV1LocalEducationAgency.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_local_education_agency_created_response import EdfiAdminApiEdfiAdminV1LocalEducationAgencyCreatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1LocalEducationAgencyCreatedResponse from a JSON string
edfi_admin_api_edfi_admin_v1_local_education_agency_created_response_instance = EdfiAdminApiEdfiAdminV1LocalEducationAgencyCreatedResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1LocalEducationAgencyCreatedResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_local_education_agency_created_response_dict = edfi_admin_api_edfi_admin_v1_local_education_agency_created_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1LocalEducationAgencyCreatedResponse from a dict
edfi_admin_api_edfi_admin_v1_local_education_agency_created_response_from_dict = EdfiAdminApiEdfiAdminV1LocalEducationAgencyCreatedResponse.from_dict(edfi_admin_api_edfi_admin_v1_local_education_agency_created_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


