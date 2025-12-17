# FormApiFormsV1UpdateFullQuestionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**type** | [**FormApiQuestionsV1QuestionType**](FormApiQuestionsV1QuestionType.md) |  | [optional] 
**required** | **bool** |  | [optional] 
**default_value** | **str** |  | [optional] 
**validation** | [**FormApiFormsV1UpdateFullQuestionValidationRequest**](FormApiFormsV1UpdateFullQuestionValidationRequest.md) |  | [optional] 
**options** | **List[str]** |  | [optional] [readonly] 
**order** | **int** |  | [optional] 
**component** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_forms_v1_update_full_question_request import FormApiFormsV1UpdateFullQuestionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiFormsV1UpdateFullQuestionRequest from a JSON string
form_api_forms_v1_update_full_question_request_instance = FormApiFormsV1UpdateFullQuestionRequest.from_json(json)
# print the JSON string representation of the object
print(FormApiFormsV1UpdateFullQuestionRequest.to_json())

# convert the object into a dict
form_api_forms_v1_update_full_question_request_dict = form_api_forms_v1_update_full_question_request_instance.to_dict()
# create an instance of FormApiFormsV1UpdateFullQuestionRequest from a dict
form_api_forms_v1_update_full_question_request_from_dict = FormApiFormsV1UpdateFullQuestionRequest.from_dict(form_api_forms_v1_update_full_question_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


