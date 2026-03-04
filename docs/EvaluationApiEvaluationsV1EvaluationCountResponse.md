# EvaluationApiEvaluationsV1EvaluationCountResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**evaluation_count** | **int** |  | [optional] 
**appraiser_count** | **int** |  | [optional] 
**staff_count** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.evaluation_api_evaluations_v1_evaluation_count_response import EvaluationApiEvaluationsV1EvaluationCountResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EvaluationApiEvaluationsV1EvaluationCountResponse from a JSON string
evaluation_api_evaluations_v1_evaluation_count_response_instance = EvaluationApiEvaluationsV1EvaluationCountResponse.from_json(json)
# print the JSON string representation of the object
print(EvaluationApiEvaluationsV1EvaluationCountResponse.to_json())

# convert the object into a dict
evaluation_api_evaluations_v1_evaluation_count_response_dict = evaluation_api_evaluations_v1_evaluation_count_response_instance.to_dict()
# create an instance of EvaluationApiEvaluationsV1EvaluationCountResponse from a dict
evaluation_api_evaluations_v1_evaluation_count_response_from_dict = EvaluationApiEvaluationsV1EvaluationCountResponse.from_dict(evaluation_api_evaluations_v1_evaluation_count_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


