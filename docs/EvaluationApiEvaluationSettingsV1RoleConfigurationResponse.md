# EvaluationApiEvaluationSettingsV1RoleConfigurationResponse

Role Personas

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**role** | **str** |  | [optional] 
**assigned_persona_identifiers** | **List[str]** |  | [optional] [readonly] 
**ignore_organization** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.evaluation_api_evaluation_settings_v1_role_configuration_response import EvaluationApiEvaluationSettingsV1RoleConfigurationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EvaluationApiEvaluationSettingsV1RoleConfigurationResponse from a JSON string
evaluation_api_evaluation_settings_v1_role_configuration_response_instance = EvaluationApiEvaluationSettingsV1RoleConfigurationResponse.from_json(json)
# print the JSON string representation of the object
print(EvaluationApiEvaluationSettingsV1RoleConfigurationResponse.to_json())

# convert the object into a dict
evaluation_api_evaluation_settings_v1_role_configuration_response_dict = evaluation_api_evaluation_settings_v1_role_configuration_response_instance.to_dict()
# create an instance of EvaluationApiEvaluationSettingsV1RoleConfigurationResponse from a dict
evaluation_api_evaluation_settings_v1_role_configuration_response_from_dict = EvaluationApiEvaluationSettingsV1RoleConfigurationResponse.from_dict(evaluation_api_evaluation_settings_v1_role_configuration_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


