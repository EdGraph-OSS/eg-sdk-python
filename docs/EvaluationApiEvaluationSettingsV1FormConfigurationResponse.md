# EvaluationApiEvaluationSettingsV1FormConfigurationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**form_id** | **str** |  | [optional] 
**versions** | [**List[EvaluationApiEvaluationSettingsV1FormVersionConfigurationResponse]**](EvaluationApiEvaluationSettingsV1FormVersionConfigurationResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.evaluation_api_evaluation_settings_v1_form_configuration_response import EvaluationApiEvaluationSettingsV1FormConfigurationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EvaluationApiEvaluationSettingsV1FormConfigurationResponse from a JSON string
evaluation_api_evaluation_settings_v1_form_configuration_response_instance = EvaluationApiEvaluationSettingsV1FormConfigurationResponse.from_json(json)
# print the JSON string representation of the object
print(EvaluationApiEvaluationSettingsV1FormConfigurationResponse.to_json())

# convert the object into a dict
evaluation_api_evaluation_settings_v1_form_configuration_response_dict = evaluation_api_evaluation_settings_v1_form_configuration_response_instance.to_dict()
# create an instance of EvaluationApiEvaluationSettingsV1FormConfigurationResponse from a dict
evaluation_api_evaluation_settings_v1_form_configuration_response_from_dict = EvaluationApiEvaluationSettingsV1FormConfigurationResponse.from_dict(evaluation_api_evaluation_settings_v1_form_configuration_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


