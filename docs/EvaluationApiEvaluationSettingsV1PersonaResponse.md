# EvaluationApiEvaluationSettingsV1PersonaResponse

Available Personas

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**identifier** | **str** |  | [optional] 
**is_default** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.evaluation_api_evaluation_settings_v1_persona_response import EvaluationApiEvaluationSettingsV1PersonaResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EvaluationApiEvaluationSettingsV1PersonaResponse from a JSON string
evaluation_api_evaluation_settings_v1_persona_response_instance = EvaluationApiEvaluationSettingsV1PersonaResponse.from_json(json)
# print the JSON string representation of the object
print(EvaluationApiEvaluationSettingsV1PersonaResponse.to_json())

# convert the object into a dict
evaluation_api_evaluation_settings_v1_persona_response_dict = evaluation_api_evaluation_settings_v1_persona_response_instance.to_dict()
# create an instance of EvaluationApiEvaluationSettingsV1PersonaResponse from a dict
evaluation_api_evaluation_settings_v1_persona_response_from_dict = EvaluationApiEvaluationSettingsV1PersonaResponse.from_dict(evaluation_api_evaluation_settings_v1_persona_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


