# FormApiFormsV1CreateFullQuestionValidationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**min_length** | **int** |  | [optional] 
**max_length** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_forms_v1_create_full_question_validation_request import FormApiFormsV1CreateFullQuestionValidationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiFormsV1CreateFullQuestionValidationRequest from a JSON string
form_api_forms_v1_create_full_question_validation_request_instance = FormApiFormsV1CreateFullQuestionValidationRequest.from_json(json)
# print the JSON string representation of the object
print(FormApiFormsV1CreateFullQuestionValidationRequest.to_json())

# convert the object into a dict
form_api_forms_v1_create_full_question_validation_request_dict = form_api_forms_v1_create_full_question_validation_request_instance.to_dict()
# create an instance of FormApiFormsV1CreateFullQuestionValidationRequest from a dict
form_api_forms_v1_create_full_question_validation_request_from_dict = FormApiFormsV1CreateFullQuestionValidationRequest.from_dict(form_api_forms_v1_create_full_question_validation_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


