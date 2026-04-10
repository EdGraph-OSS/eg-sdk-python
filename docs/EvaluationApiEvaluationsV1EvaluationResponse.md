# EvaluationApiEvaluationsV1EvaluationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**evaluation_date** | **str** |  | [optional] 
**submission_date** | **str** |  | [optional] 
**campus** | **str** |  | [optional] 
**appraiser_user_id** | **str** |  | [optional] 
**staff_user_id** | **str** |  | [optional] 
**form_id** | **str** |  | [optional] 
**form_version** | **str** |  | [optional] 
**status** | [**EvaluationApiEvaluationsV1EvaluationStatus**](EvaluationApiEvaluationsV1EvaluationStatus.md) |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**appraiser_full_name** | **str** |  | [optional] 
**staff_full_name** | **str** |  | [optional] 
**campus_class_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.evaluation_api_evaluations_v1_evaluation_response import EvaluationApiEvaluationsV1EvaluationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EvaluationApiEvaluationsV1EvaluationResponse from a JSON string
evaluation_api_evaluations_v1_evaluation_response_instance = EvaluationApiEvaluationsV1EvaluationResponse.from_json(json)
# print the JSON string representation of the object
print(EvaluationApiEvaluationsV1EvaluationResponse.to_json())

# convert the object into a dict
evaluation_api_evaluations_v1_evaluation_response_dict = evaluation_api_evaluations_v1_evaluation_response_instance.to_dict()
# create an instance of EvaluationApiEvaluationsV1EvaluationResponse from a dict
evaluation_api_evaluations_v1_evaluation_response_from_dict = EvaluationApiEvaluationsV1EvaluationResponse.from_dict(evaluation_api_evaluations_v1_evaluation_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


