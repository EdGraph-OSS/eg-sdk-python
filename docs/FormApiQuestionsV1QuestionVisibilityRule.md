# FormApiQuestionsV1QuestionVisibilityRule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**field_id** | **str** |  | [optional] 
**operator** | **str** |  | [optional] 
**value** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_questions_v1_question_visibility_rule import FormApiQuestionsV1QuestionVisibilityRule

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiQuestionsV1QuestionVisibilityRule from a JSON string
form_api_questions_v1_question_visibility_rule_instance = FormApiQuestionsV1QuestionVisibilityRule.from_json(json)
# print the JSON string representation of the object
print(FormApiQuestionsV1QuestionVisibilityRule.to_json())

# convert the object into a dict
form_api_questions_v1_question_visibility_rule_dict = form_api_questions_v1_question_visibility_rule_instance.to_dict()
# create an instance of FormApiQuestionsV1QuestionVisibilityRule from a dict
form_api_questions_v1_question_visibility_rule_from_dict = FormApiQuestionsV1QuestionVisibilityRule.from_dict(form_api_questions_v1_question_visibility_rule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


