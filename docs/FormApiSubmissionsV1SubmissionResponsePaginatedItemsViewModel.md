# FormApiSubmissionsV1SubmissionResponsePaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[FormApiSubmissionsV1SubmissionResponse]**](FormApiSubmissionsV1SubmissionResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_submissions_v1_submission_response_paginated_items_view_model import FormApiSubmissionsV1SubmissionResponsePaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiSubmissionsV1SubmissionResponsePaginatedItemsViewModel from a JSON string
form_api_submissions_v1_submission_response_paginated_items_view_model_instance = FormApiSubmissionsV1SubmissionResponsePaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(FormApiSubmissionsV1SubmissionResponsePaginatedItemsViewModel.to_json())

# convert the object into a dict
form_api_submissions_v1_submission_response_paginated_items_view_model_dict = form_api_submissions_v1_submission_response_paginated_items_view_model_instance.to_dict()
# create an instance of FormApiSubmissionsV1SubmissionResponsePaginatedItemsViewModel from a dict
form_api_submissions_v1_submission_response_paginated_items_view_model_from_dict = FormApiSubmissionsV1SubmissionResponsePaginatedItemsViewModel.from_dict(form_api_submissions_v1_submission_response_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


