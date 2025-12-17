# IdentityApiUserV1EducationOrganizationRemovedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**education_organization_id** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_education_organization_removed_response import IdentityApiUserV1EducationOrganizationRemovedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1EducationOrganizationRemovedResponse from a JSON string
identity_api_user_v1_education_organization_removed_response_instance = IdentityApiUserV1EducationOrganizationRemovedResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1EducationOrganizationRemovedResponse.to_json())

# convert the object into a dict
identity_api_user_v1_education_organization_removed_response_dict = identity_api_user_v1_education_organization_removed_response_instance.to_dict()
# create an instance of IdentityApiUserV1EducationOrganizationRemovedResponse from a dict
identity_api_user_v1_education_organization_removed_response_from_dict = IdentityApiUserV1EducationOrganizationRemovedResponse.from_dict(identity_api_user_v1_education_organization_removed_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


