# ValidationsApiJobsV1PaginatedItemsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[ValidationsApiJobsV1JobListResponse]**](ValidationsApiJobsV1JobListResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_jobs_v1_paginated_items_response import ValidationsApiJobsV1PaginatedItemsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiJobsV1PaginatedItemsResponse from a JSON string
validations_api_jobs_v1_paginated_items_response_instance = ValidationsApiJobsV1PaginatedItemsResponse.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiJobsV1PaginatedItemsResponse.to_json())

# convert the object into a dict
validations_api_jobs_v1_paginated_items_response_dict = validations_api_jobs_v1_paginated_items_response_instance.to_dict()
# create an instance of ValidationsApiJobsV1PaginatedItemsResponse from a dict
validations_api_jobs_v1_paginated_items_response_from_dict = ValidationsApiJobsV1PaginatedItemsResponse.from_dict(validations_api_jobs_v1_paginated_items_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


