# IdentityApiUserV1EducationOrganization


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**education_organization_id** | **int** |  | [optional] 
**short_name_of_institution** | **str** |  | [optional] 
**name_of_institution** | **str** |  | [optional] 
**staff_classifications** | **List[str]** |  | [optional] [readonly] 
**source** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_education_organization import IdentityApiUserV1EducationOrganization

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1EducationOrganization from a JSON string
identity_api_user_v1_education_organization_instance = IdentityApiUserV1EducationOrganization.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1EducationOrganization.to_json())

# convert the object into a dict
identity_api_user_v1_education_organization_dict = identity_api_user_v1_education_organization_instance.to_dict()
# create an instance of IdentityApiUserV1EducationOrganization from a dict
identity_api_user_v1_education_organization_from_dict = IdentityApiUserV1EducationOrganization.from_dict(identity_api_user_v1_education_organization_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


