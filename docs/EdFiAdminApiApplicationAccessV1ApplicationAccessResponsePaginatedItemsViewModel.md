# EdFiAdminApiApplicationAccessV1ApplicationAccessResponsePaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EdFiAdminApiApplicationAccessV1ApplicationAccessResponse]**](EdFiAdminApiApplicationAccessV1ApplicationAccessResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_fi_admin_api_application_access_v1_application_access_response_paginated_items_view_model import EdFiAdminApiApplicationAccessV1ApplicationAccessResponsePaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of EdFiAdminApiApplicationAccessV1ApplicationAccessResponsePaginatedItemsViewModel from a JSON string
ed_fi_admin_api_application_access_v1_application_access_response_paginated_items_view_model_instance = EdFiAdminApiApplicationAccessV1ApplicationAccessResponsePaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(EdFiAdminApiApplicationAccessV1ApplicationAccessResponsePaginatedItemsViewModel.to_json())

# convert the object into a dict
ed_fi_admin_api_application_access_v1_application_access_response_paginated_items_view_model_dict = ed_fi_admin_api_application_access_v1_application_access_response_paginated_items_view_model_instance.to_dict()
# create an instance of EdFiAdminApiApplicationAccessV1ApplicationAccessResponsePaginatedItemsViewModel from a dict
ed_fi_admin_api_application_access_v1_application_access_response_paginated_items_view_model_from_dict = EdFiAdminApiApplicationAccessV1ApplicationAccessResponsePaginatedItemsViewModel.from_dict(ed_fi_admin_api_application_access_v1_application_access_response_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


