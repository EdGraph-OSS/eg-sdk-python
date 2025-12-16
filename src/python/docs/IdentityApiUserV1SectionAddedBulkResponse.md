# IdentityApiUserV1SectionAddedBulkResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_section_added_bulk_response import IdentityApiUserV1SectionAddedBulkResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1SectionAddedBulkResponse from a JSON string
identity_api_user_v1_section_added_bulk_response_instance = IdentityApiUserV1SectionAddedBulkResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1SectionAddedBulkResponse.to_json())

# convert the object into a dict
identity_api_user_v1_section_added_bulk_response_dict = identity_api_user_v1_section_added_bulk_response_instance.to_dict()
# create an instance of IdentityApiUserV1SectionAddedBulkResponse from a dict
identity_api_user_v1_section_added_bulk_response_from_dict = IdentityApiUserV1SectionAddedBulkResponse.from_dict(identity_api_user_v1_section_added_bulk_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


