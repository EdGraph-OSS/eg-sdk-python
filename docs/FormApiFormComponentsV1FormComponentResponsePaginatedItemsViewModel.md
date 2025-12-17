# FormApiFormComponentsV1FormComponentResponsePaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[FormApiFormComponentsV1FormComponentResponse]**](FormApiFormComponentsV1FormComponentResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_form_components_v1_form_component_response_paginated_items_view_model import FormApiFormComponentsV1FormComponentResponsePaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiFormComponentsV1FormComponentResponsePaginatedItemsViewModel from a JSON string
form_api_form_components_v1_form_component_response_paginated_items_view_model_instance = FormApiFormComponentsV1FormComponentResponsePaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(FormApiFormComponentsV1FormComponentResponsePaginatedItemsViewModel.to_json())

# convert the object into a dict
form_api_form_components_v1_form_component_response_paginated_items_view_model_dict = form_api_form_components_v1_form_component_response_paginated_items_view_model_instance.to_dict()
# create an instance of FormApiFormComponentsV1FormComponentResponsePaginatedItemsViewModel from a dict
form_api_form_components_v1_form_component_response_paginated_items_view_model_from_dict = FormApiFormComponentsV1FormComponentResponsePaginatedItemsViewModel.from_dict(form_api_form_components_v1_form_component_response_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


