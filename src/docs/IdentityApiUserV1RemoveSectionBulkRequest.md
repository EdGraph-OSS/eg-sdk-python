# IdentityApiUserV1RemoveSectionBulkRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**user_section_ids** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_remove_section_bulk_request import IdentityApiUserV1RemoveSectionBulkRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1RemoveSectionBulkRequest from a JSON string
identity_api_user_v1_remove_section_bulk_request_instance = IdentityApiUserV1RemoveSectionBulkRequest.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1RemoveSectionBulkRequest.to_json())

# convert the object into a dict
identity_api_user_v1_remove_section_bulk_request_dict = identity_api_user_v1_remove_section_bulk_request_instance.to_dict()
# create an instance of IdentityApiUserV1RemoveSectionBulkRequest from a dict
identity_api_user_v1_remove_section_bulk_request_from_dict = IdentityApiUserV1RemoveSectionBulkRequest.from_dict(identity_api_user_v1_remove_section_bulk_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


