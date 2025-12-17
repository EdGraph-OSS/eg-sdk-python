# FormApiQuestionsV1QuestionUpdatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**form_id** | **str** |  | [optional] 
**section_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_questions_v1_question_updated_response import FormApiQuestionsV1QuestionUpdatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiQuestionsV1QuestionUpdatedResponse from a JSON string
form_api_questions_v1_question_updated_response_instance = FormApiQuestionsV1QuestionUpdatedResponse.from_json(json)
# print the JSON string representation of the object
print(FormApiQuestionsV1QuestionUpdatedResponse.to_json())

# convert the object into a dict
form_api_questions_v1_question_updated_response_dict = form_api_questions_v1_question_updated_response_instance.to_dict()
# create an instance of FormApiQuestionsV1QuestionUpdatedResponse from a dict
form_api_questions_v1_question_updated_response_from_dict = FormApiQuestionsV1QuestionUpdatedResponse.from_dict(form_api_questions_v1_question_updated_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


