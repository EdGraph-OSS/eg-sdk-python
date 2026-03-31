# FormApiQuestionsV1QuestionVisibilityCondition


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**logic** | **str** |  | [optional] 
**rules** | [**List[FormApiQuestionsV1QuestionVisibilityRule]**](FormApiQuestionsV1QuestionVisibilityRule.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.form_api_questions_v1_question_visibility_condition import FormApiQuestionsV1QuestionVisibilityCondition

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiQuestionsV1QuestionVisibilityCondition from a JSON string
form_api_questions_v1_question_visibility_condition_instance = FormApiQuestionsV1QuestionVisibilityCondition.from_json(json)
# print the JSON string representation of the object
print(FormApiQuestionsV1QuestionVisibilityCondition.to_json())

# convert the object into a dict
form_api_questions_v1_question_visibility_condition_dict = form_api_questions_v1_question_visibility_condition_instance.to_dict()
# create an instance of FormApiQuestionsV1QuestionVisibilityCondition from a dict
form_api_questions_v1_question_visibility_condition_from_dict = FormApiQuestionsV1QuestionVisibilityCondition.from_dict(form_api_questions_v1_question_visibility_condition_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


