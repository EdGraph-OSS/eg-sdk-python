# ValidationsApiTagsV1PaginatedTags


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[ValidationsApiTagsV1TagDto]**](ValidationsApiTagsV1TagDto.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_tags_v1_paginated_tags import ValidationsApiTagsV1PaginatedTags

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiTagsV1PaginatedTags from a JSON string
validations_api_tags_v1_paginated_tags_instance = ValidationsApiTagsV1PaginatedTags.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiTagsV1PaginatedTags.to_json())

# convert the object into a dict
validations_api_tags_v1_paginated_tags_dict = validations_api_tags_v1_paginated_tags_instance.to_dict()
# create an instance of ValidationsApiTagsV1PaginatedTags from a dict
validations_api_tags_v1_paginated_tags_from_dict = ValidationsApiTagsV1PaginatedTags.from_dict(validations_api_tags_v1_paginated_tags_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


