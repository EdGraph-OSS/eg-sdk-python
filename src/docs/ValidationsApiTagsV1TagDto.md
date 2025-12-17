# ValidationsApiTagsV1TagDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**is_public** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_tags_v1_tag_dto import ValidationsApiTagsV1TagDto

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiTagsV1TagDto from a JSON string
validations_api_tags_v1_tag_dto_instance = ValidationsApiTagsV1TagDto.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiTagsV1TagDto.to_json())

# convert the object into a dict
validations_api_tags_v1_tag_dto_dict = validations_api_tags_v1_tag_dto_instance.to_dict()
# create an instance of ValidationsApiTagsV1TagDto from a dict
validations_api_tags_v1_tag_dto_from_dict = ValidationsApiTagsV1TagDto.from_dict(validations_api_tags_v1_tag_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


