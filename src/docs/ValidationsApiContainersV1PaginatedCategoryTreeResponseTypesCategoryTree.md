# ValidationsApiContainersV1PaginatedCategoryTreeResponseTypesCategoryTree


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**category_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**sub_categories** | [**List[ValidationsApiContainersV1PaginatedCategoryTreeResponseTypesSubCategoryTree]**](ValidationsApiContainersV1PaginatedCategoryTreeResponseTypesSubCategoryTree.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_containers_v1_paginated_category_tree_response_types_category_tree import ValidationsApiContainersV1PaginatedCategoryTreeResponseTypesCategoryTree

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiContainersV1PaginatedCategoryTreeResponseTypesCategoryTree from a JSON string
validations_api_containers_v1_paginated_category_tree_response_types_category_tree_instance = ValidationsApiContainersV1PaginatedCategoryTreeResponseTypesCategoryTree.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiContainersV1PaginatedCategoryTreeResponseTypesCategoryTree.to_json())

# convert the object into a dict
validations_api_containers_v1_paginated_category_tree_response_types_category_tree_dict = validations_api_containers_v1_paginated_category_tree_response_types_category_tree_instance.to_dict()
# create an instance of ValidationsApiContainersV1PaginatedCategoryTreeResponseTypesCategoryTree from a dict
validations_api_containers_v1_paginated_category_tree_response_types_category_tree_from_dict = ValidationsApiContainersV1PaginatedCategoryTreeResponseTypesCategoryTree.from_dict(validations_api_containers_v1_paginated_category_tree_response_types_category_tree_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


