# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsCreateQuestionRequestDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**form_id** | **str** |  | [optional] 
**section_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**type** | [**FormApiQuestionsV1QuestionType**](FormApiQuestionsV1QuestionType.md) |  | [optional] 
**required** | **bool** |  | [optional] 
**default_value** | **str** |  | [optional] 
**validation** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsCreateQuestionValidationRequestDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsCreateQuestionValidationRequestDto.md) |  | [optional] 
**options** | **List[str]** |  | [optional] 
**order** | **int** |  | [optional] 
**component** | **object** |  | [optional] 
**visibility_condition** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesFormsQuestionVisibilityConditionDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesFormsQuestionVisibilityConditionDto.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_create_question_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsCreateQuestionRequestDto

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsCreateQuestionRequestDto from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_create_question_request_dto_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsCreateQuestionRequestDto.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsCreateQuestionRequestDto.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_create_question_request_dto_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_create_question_request_dto_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsCreateQuestionRequestDto from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_create_question_request_dto_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsFormsCreateQuestionRequestDto.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_forms_create_question_request_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


