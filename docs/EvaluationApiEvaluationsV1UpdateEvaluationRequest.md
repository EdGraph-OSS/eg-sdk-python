# EvaluationApiEvaluationsV1UpdateEvaluationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**evaluation_date** | **str** |  | [optional] 
**campus** | **str** |  | [optional] 
**appraiser_user_id** | **str** |  | [optional] 
**staff_user_id** | **str** |  | [optional] 
**form_id** | **str** |  | [optional] 
**form_version** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.evaluation_api_evaluations_v1_update_evaluation_request import EvaluationApiEvaluationsV1UpdateEvaluationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EvaluationApiEvaluationsV1UpdateEvaluationRequest from a JSON string
evaluation_api_evaluations_v1_update_evaluation_request_instance = EvaluationApiEvaluationsV1UpdateEvaluationRequest.from_json(json)
# print the JSON string representation of the object
print(EvaluationApiEvaluationsV1UpdateEvaluationRequest.to_json())

# convert the object into a dict
evaluation_api_evaluations_v1_update_evaluation_request_dict = evaluation_api_evaluations_v1_update_evaluation_request_instance.to_dict()
# create an instance of EvaluationApiEvaluationsV1UpdateEvaluationRequest from a dict
evaluation_api_evaluations_v1_update_evaluation_request_from_dict = EvaluationApiEvaluationsV1UpdateEvaluationRequest.from_dict(evaluation_api_evaluations_v1_update_evaluation_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


