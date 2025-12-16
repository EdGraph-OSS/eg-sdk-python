# ApplicationApiApplicationV1PaginatedItemsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[ApplicationApiApplicationV1ApplicationListResponse]**](ApplicationApiApplicationV1ApplicationListResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.application_api_application_v1_paginated_items_response import ApplicationApiApplicationV1PaginatedItemsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ApplicationApiApplicationV1PaginatedItemsResponse from a JSON string
application_api_application_v1_paginated_items_response_instance = ApplicationApiApplicationV1PaginatedItemsResponse.from_json(json)
# print the JSON string representation of the object
print(ApplicationApiApplicationV1PaginatedItemsResponse.to_json())

# convert the object into a dict
application_api_application_v1_paginated_items_response_dict = application_api_application_v1_paginated_items_response_instance.to_dict()
# create an instance of ApplicationApiApplicationV1PaginatedItemsResponse from a dict
application_api_application_v1_paginated_items_response_from_dict = ApplicationApiApplicationV1PaginatedItemsResponse.from_dict(application_api_application_v1_paginated_items_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


