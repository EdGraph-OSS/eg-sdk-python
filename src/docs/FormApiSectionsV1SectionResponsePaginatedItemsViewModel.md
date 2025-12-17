# FormApiSectionsV1SectionResponsePaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[FormApiSectionsV1SectionResponse]**](FormApiSectionsV1SectionResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_sections_v1_section_response_paginated_items_view_model import FormApiSectionsV1SectionResponsePaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiSectionsV1SectionResponsePaginatedItemsViewModel from a JSON string
form_api_sections_v1_section_response_paginated_items_view_model_instance = FormApiSectionsV1SectionResponsePaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(FormApiSectionsV1SectionResponsePaginatedItemsViewModel.to_json())

# convert the object into a dict
form_api_sections_v1_section_response_paginated_items_view_model_dict = form_api_sections_v1_section_response_paginated_items_view_model_instance.to_dict()
# create an instance of FormApiSectionsV1SectionResponsePaginatedItemsViewModel from a dict
form_api_sections_v1_section_response_paginated_items_view_model_from_dict = FormApiSectionsV1SectionResponsePaginatedItemsViewModel.from_dict(form_api_sections_v1_section_response_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


