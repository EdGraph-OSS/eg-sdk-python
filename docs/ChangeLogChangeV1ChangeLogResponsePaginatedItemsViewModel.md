# ChangeLogChangeV1ChangeLogResponsePaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[ChangeLogChangeV1ChangeLogResponse]**](ChangeLogChangeV1ChangeLogResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.change_log_change_v1_change_log_response_paginated_items_view_model import ChangeLogChangeV1ChangeLogResponsePaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of ChangeLogChangeV1ChangeLogResponsePaginatedItemsViewModel from a JSON string
change_log_change_v1_change_log_response_paginated_items_view_model_instance = ChangeLogChangeV1ChangeLogResponsePaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(ChangeLogChangeV1ChangeLogResponsePaginatedItemsViewModel.to_json())

# convert the object into a dict
change_log_change_v1_change_log_response_paginated_items_view_model_dict = change_log_change_v1_change_log_response_paginated_items_view_model_instance.to_dict()
# create an instance of ChangeLogChangeV1ChangeLogResponsePaginatedItemsViewModel from a dict
change_log_change_v1_change_log_response_paginated_items_view_model_from_dict = ChangeLogChangeV1ChangeLogResponsePaginatedItemsViewModel.from_dict(change_log_change_v1_change_log_response_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


