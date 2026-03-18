# EvaluationApiEvaluationSettingsV1FormVersionConfigurationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**version** | **str** |  | [optional] 
**active_starting_date** | **str** |  | [optional] 
**active_until_date** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.evaluation_api_evaluation_settings_v1_form_version_configuration_response import EvaluationApiEvaluationSettingsV1FormVersionConfigurationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EvaluationApiEvaluationSettingsV1FormVersionConfigurationResponse from a JSON string
evaluation_api_evaluation_settings_v1_form_version_configuration_response_instance = EvaluationApiEvaluationSettingsV1FormVersionConfigurationResponse.from_json(json)
# print the JSON string representation of the object
print(EvaluationApiEvaluationSettingsV1FormVersionConfigurationResponse.to_json())

# convert the object into a dict
evaluation_api_evaluation_settings_v1_form_version_configuration_response_dict = evaluation_api_evaluation_settings_v1_form_version_configuration_response_instance.to_dict()
# create an instance of EvaluationApiEvaluationSettingsV1FormVersionConfigurationResponse from a dict
evaluation_api_evaluation_settings_v1_form_version_configuration_response_from_dict = EvaluationApiEvaluationSettingsV1FormVersionConfigurationResponse.from_dict(evaluation_api_evaluation_settings_v1_form_version_configuration_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


