# IdentityApiUserV1AddSectionBulkRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**sections** | [**List[IdentityApiUserV1AddSectionBulkRequestTypesSectionDto]**](IdentityApiUserV1AddSectionBulkRequestTypesSectionDto.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_add_section_bulk_request import IdentityApiUserV1AddSectionBulkRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1AddSectionBulkRequest from a JSON string
identity_api_user_v1_add_section_bulk_request_instance = IdentityApiUserV1AddSectionBulkRequest.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1AddSectionBulkRequest.to_json())

# convert the object into a dict
identity_api_user_v1_add_section_bulk_request_dict = identity_api_user_v1_add_section_bulk_request_instance.to_dict()
# create an instance of IdentityApiUserV1AddSectionBulkRequest from a dict
identity_api_user_v1_add_section_bulk_request_from_dict = IdentityApiUserV1AddSectionBulkRequest.from_dict(identity_api_user_v1_add_section_bulk_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


