# EvaluationApiEvaluationSettingsV1SetFormConfigurationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**form_id** | **str** |  | [optional] 
**versions** | [**List[EvaluationApiEvaluationSettingsV1SetFormVersionConfigurationRequest]**](EvaluationApiEvaluationSettingsV1SetFormVersionConfigurationRequest.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.evaluation_api_evaluation_settings_v1_set_form_configuration_request import EvaluationApiEvaluationSettingsV1SetFormConfigurationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EvaluationApiEvaluationSettingsV1SetFormConfigurationRequest from a JSON string
evaluation_api_evaluation_settings_v1_set_form_configuration_request_instance = EvaluationApiEvaluationSettingsV1SetFormConfigurationRequest.from_json(json)
# print the JSON string representation of the object
print(EvaluationApiEvaluationSettingsV1SetFormConfigurationRequest.to_json())

# convert the object into a dict
evaluation_api_evaluation_settings_v1_set_form_configuration_request_dict = evaluation_api_evaluation_settings_v1_set_form_configuration_request_instance.to_dict()
# create an instance of EvaluationApiEvaluationSettingsV1SetFormConfigurationRequest from a dict
evaluation_api_evaluation_settings_v1_set_form_configuration_request_from_dict = EvaluationApiEvaluationSettingsV1SetFormConfigurationRequest.from_dict(evaluation_api_evaluation_settings_v1_set_form_configuration_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


