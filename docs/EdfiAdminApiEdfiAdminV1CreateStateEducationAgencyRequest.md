# EdfiAdminApiEdfiAdminV1CreateStateEducationAgencyRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**state_education_agency_id** | **int** |  | [optional] 
**name_of_institution** | **str** |  | [optional] 
**education_organization_category_descriptors** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_state_education_agency_request import EdfiAdminApiEdfiAdminV1CreateStateEducationAgencyRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1CreateStateEducationAgencyRequest from a JSON string
edfi_admin_api_edfi_admin_v1_create_state_education_agency_request_instance = EdfiAdminApiEdfiAdminV1CreateStateEducationAgencyRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1CreateStateEducationAgencyRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_create_state_education_agency_request_dict = edfi_admin_api_edfi_admin_v1_create_state_education_agency_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1CreateStateEducationAgencyRequest from a dict
edfi_admin_api_edfi_admin_v1_create_state_education_agency_request_from_dict = EdfiAdminApiEdfiAdminV1CreateStateEducationAgencyRequest.from_dict(edfi_admin_api_edfi_admin_v1_create_state_education_agency_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


