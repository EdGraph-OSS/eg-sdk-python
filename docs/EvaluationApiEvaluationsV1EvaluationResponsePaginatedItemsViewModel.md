# EvaluationApiEvaluationsV1EvaluationResponsePaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EvaluationApiEvaluationsV1EvaluationResponse]**](EvaluationApiEvaluationsV1EvaluationResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.evaluation_api_evaluations_v1_evaluation_response_paginated_items_view_model import EvaluationApiEvaluationsV1EvaluationResponsePaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of EvaluationApiEvaluationsV1EvaluationResponsePaginatedItemsViewModel from a JSON string
evaluation_api_evaluations_v1_evaluation_response_paginated_items_view_model_instance = EvaluationApiEvaluationsV1EvaluationResponsePaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(EvaluationApiEvaluationsV1EvaluationResponsePaginatedItemsViewModel.to_json())

# convert the object into a dict
evaluation_api_evaluations_v1_evaluation_response_paginated_items_view_model_dict = evaluation_api_evaluations_v1_evaluation_response_paginated_items_view_model_instance.to_dict()
# create an instance of EvaluationApiEvaluationsV1EvaluationResponsePaginatedItemsViewModel from a dict
evaluation_api_evaluations_v1_evaluation_response_paginated_items_view_model_from_dict = EvaluationApiEvaluationsV1EvaluationResponsePaginatedItemsViewModel.from_dict(evaluation_api_evaluations_v1_evaluation_response_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


