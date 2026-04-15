# FormApiFormsV1CreateFullQuestionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**type** | [**FormApiQuestionsV1QuestionType**](FormApiQuestionsV1QuestionType.md) |  | [optional] 
**required** | **bool** |  | [optional] 
**default_value** | **str** |  | [optional] 
**validation** | [**FormApiFormsV1CreateFullQuestionValidationRequest**](FormApiFormsV1CreateFullQuestionValidationRequest.md) |  | [optional] 
**options** | **List[str]** |  | [optional] [readonly] 
**order** | **int** |  | [optional] 
**component** | **str** |  | [optional] 
**custom_id** | **str** |  | [optional] 
**visibility_condition** | [**FormApiQuestionsV1QuestionVisibilityCondition**](FormApiQuestionsV1QuestionVisibilityCondition.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_forms_v1_create_full_question_request import FormApiFormsV1CreateFullQuestionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiFormsV1CreateFullQuestionRequest from a JSON string
form_api_forms_v1_create_full_question_request_instance = FormApiFormsV1CreateFullQuestionRequest.from_json(json)
# print the JSON string representation of the object
print(FormApiFormsV1CreateFullQuestionRequest.to_json())

# convert the object into a dict
form_api_forms_v1_create_full_question_request_dict = form_api_forms_v1_create_full_question_request_instance.to_dict()
# create an instance of FormApiFormsV1CreateFullQuestionRequest from a dict
form_api_forms_v1_create_full_question_request_from_dict = FormApiFormsV1CreateFullQuestionRequest.from_dict(form_api_forms_v1_create_full_question_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


