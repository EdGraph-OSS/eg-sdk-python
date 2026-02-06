# EvaluationApiEvaluationSettingsV1SetApplicationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**forms** | **List[str]** |  | [optional] [readonly] 
**recommended_number_of_evaluations** | **int** |  | [optional] 
**reminder_email_schedule** | [**EvaluationApiEvaluationSettingsV1ScheduleType**](EvaluationApiEvaluationSettingsV1ScheduleType.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.evaluation_api_evaluation_settings_v1_set_application_request import EvaluationApiEvaluationSettingsV1SetApplicationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EvaluationApiEvaluationSettingsV1SetApplicationRequest from a JSON string
evaluation_api_evaluation_settings_v1_set_application_request_instance = EvaluationApiEvaluationSettingsV1SetApplicationRequest.from_json(json)
# print the JSON string representation of the object
print(EvaluationApiEvaluationSettingsV1SetApplicationRequest.to_json())

# convert the object into a dict
evaluation_api_evaluation_settings_v1_set_application_request_dict = evaluation_api_evaluation_settings_v1_set_application_request_instance.to_dict()
# create an instance of EvaluationApiEvaluationSettingsV1SetApplicationRequest from a dict
evaluation_api_evaluation_settings_v1_set_application_request_from_dict = EvaluationApiEvaluationSettingsV1SetApplicationRequest.from_dict(evaluation_api_evaluation_settings_v1_set_application_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


