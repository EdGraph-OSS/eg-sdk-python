# IdentityApiUserV1UpdateSectionBulkRequestTypesSectionDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_section_id** | **str** |  | [optional] 
**education_organization_id** | **int** |  | [optional] 
**section_id** | **str** |  | [optional] 
**staff_unique_id** | **str** |  | [optional] 
**classroom_position_descriptor** | **str** |  | [optional] 
**begin_date** | **str** |  | [optional] 
**end_date** | **str** |  | [optional] 
**source** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_update_section_bulk_request_types_section_dto import IdentityApiUserV1UpdateSectionBulkRequestTypesSectionDto

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1UpdateSectionBulkRequestTypesSectionDto from a JSON string
identity_api_user_v1_update_section_bulk_request_types_section_dto_instance = IdentityApiUserV1UpdateSectionBulkRequestTypesSectionDto.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1UpdateSectionBulkRequestTypesSectionDto.to_json())

# convert the object into a dict
identity_api_user_v1_update_section_bulk_request_types_section_dto_dict = identity_api_user_v1_update_section_bulk_request_types_section_dto_instance.to_dict()
# create an instance of IdentityApiUserV1UpdateSectionBulkRequestTypesSectionDto from a dict
identity_api_user_v1_update_section_bulk_request_types_section_dto_from_dict = IdentityApiUserV1UpdateSectionBulkRequestTypesSectionDto.from_dict(identity_api_user_v1_update_section_bulk_request_types_section_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


