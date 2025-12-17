# EdfiAdminApiEdfiAdminV1CreateEducationServiceCenterRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**education_service_center_id** | **int** |  | [optional] 
**name_of_institution** | **str** |  | [optional] 
**education_organization_category_descriptors** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_create_education_service_center_request import EdfiAdminApiEdfiAdminV1CreateEducationServiceCenterRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1CreateEducationServiceCenterRequest from a JSON string
edfi_admin_api_edfi_admin_v1_create_education_service_center_request_instance = EdfiAdminApiEdfiAdminV1CreateEducationServiceCenterRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1CreateEducationServiceCenterRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_create_education_service_center_request_dict = edfi_admin_api_edfi_admin_v1_create_education_service_center_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1CreateEducationServiceCenterRequest from a dict
edfi_admin_api_edfi_admin_v1_create_education_service_center_request_from_dict = EdfiAdminApiEdfiAdminV1CreateEducationServiceCenterRequest.from_dict(edfi_admin_api_edfi_admin_v1_create_education_service_center_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


