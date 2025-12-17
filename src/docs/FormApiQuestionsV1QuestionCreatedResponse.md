# FormApiQuestionsV1QuestionCreatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**form_id** | **str** |  | [optional] 
**section_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_questions_v1_question_created_response import FormApiQuestionsV1QuestionCreatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiQuestionsV1QuestionCreatedResponse from a JSON string
form_api_questions_v1_question_created_response_instance = FormApiQuestionsV1QuestionCreatedResponse.from_json(json)
# print the JSON string representation of the object
print(FormApiQuestionsV1QuestionCreatedResponse.to_json())

# convert the object into a dict
form_api_questions_v1_question_created_response_dict = form_api_questions_v1_question_created_response_instance.to_dict()
# create an instance of FormApiQuestionsV1QuestionCreatedResponse from a dict
form_api_questions_v1_question_created_response_from_dict = FormApiQuestionsV1QuestionCreatedResponse.from_dict(form_api_questions_v1_question_created_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


