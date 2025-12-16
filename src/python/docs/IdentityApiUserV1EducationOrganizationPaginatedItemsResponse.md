# IdentityApiUserV1EducationOrganizationPaginatedItemsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[IdentityApiUserV1EducationOrganization]**](IdentityApiUserV1EducationOrganization.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_education_organization_paginated_items_response import IdentityApiUserV1EducationOrganizationPaginatedItemsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1EducationOrganizationPaginatedItemsResponse from a JSON string
identity_api_user_v1_education_organization_paginated_items_response_instance = IdentityApiUserV1EducationOrganizationPaginatedItemsResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1EducationOrganizationPaginatedItemsResponse.to_json())

# convert the object into a dict
identity_api_user_v1_education_organization_paginated_items_response_dict = identity_api_user_v1_education_organization_paginated_items_response_instance.to_dict()
# create an instance of IdentityApiUserV1EducationOrganizationPaginatedItemsResponse from a dict
identity_api_user_v1_education_organization_paginated_items_response_from_dict = IdentityApiUserV1EducationOrganizationPaginatedItemsResponse.from_dict(identity_api_user_v1_education_organization_paginated_items_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


