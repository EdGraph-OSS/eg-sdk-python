# EvaluationApiEvaluationsV1FormResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**version** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.evaluation_api_evaluations_v1_form_response import EvaluationApiEvaluationsV1FormResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EvaluationApiEvaluationsV1FormResponse from a JSON string
evaluation_api_evaluations_v1_form_response_instance = EvaluationApiEvaluationsV1FormResponse.from_json(json)
# print the JSON string representation of the object
print(EvaluationApiEvaluationsV1FormResponse.to_json())

# convert the object into a dict
evaluation_api_evaluations_v1_form_response_dict = evaluation_api_evaluations_v1_form_response_instance.to_dict()
# create an instance of EvaluationApiEvaluationsV1FormResponse from a dict
evaluation_api_evaluations_v1_form_response_from_dict = EvaluationApiEvaluationsV1FormResponse.from_dict(evaluation_api_evaluations_v1_form_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


