# ValidationsApiContainersV1PaginatedCategoryTreeResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[ValidationsApiContainersV1PaginatedCategoryTreeResponseTypesCategoryTree]**](ValidationsApiContainersV1PaginatedCategoryTreeResponseTypesCategoryTree.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_containers_v1_paginated_category_tree_response import ValidationsApiContainersV1PaginatedCategoryTreeResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiContainersV1PaginatedCategoryTreeResponse from a JSON string
validations_api_containers_v1_paginated_category_tree_response_instance = ValidationsApiContainersV1PaginatedCategoryTreeResponse.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiContainersV1PaginatedCategoryTreeResponse.to_json())

# convert the object into a dict
validations_api_containers_v1_paginated_category_tree_response_dict = validations_api_containers_v1_paginated_category_tree_response_instance.to_dict()
# create an instance of ValidationsApiContainersV1PaginatedCategoryTreeResponse from a dict
validations_api_containers_v1_paginated_category_tree_response_from_dict = ValidationsApiContainersV1PaginatedCategoryTreeResponse.from_dict(validations_api_containers_v1_paginated_category_tree_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


