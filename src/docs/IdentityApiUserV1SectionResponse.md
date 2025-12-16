# IdentityApiUserV1SectionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**education_organization_id** | **int** |  | [optional] 
**education_organization_name** | **str** |  | [optional] 
**section_id** | **str** |  | [optional] 
**section_identifier** | **str** |  | [optional] 
**section_name** | **str** |  | [optional] 
**staff_unique_id** | **str** |  | [optional] 
**classroom_position_descriptor** | **str** |  | [optional] 
**begin_date** | **str** |  | [optional] 
**end_date** | **str** |  | [optional] 
**source** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_section_response import IdentityApiUserV1SectionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1SectionResponse from a JSON string
identity_api_user_v1_section_response_instance = IdentityApiUserV1SectionResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1SectionResponse.to_json())

# convert the object into a dict
identity_api_user_v1_section_response_dict = identity_api_user_v1_section_response_instance.to_dict()
# create an instance of IdentityApiUserV1SectionResponse from a dict
identity_api_user_v1_section_response_from_dict = IdentityApiUserV1SectionResponse.from_dict(identity_api_user_v1_section_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


