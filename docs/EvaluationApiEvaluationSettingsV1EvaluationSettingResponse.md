# EvaluationApiEvaluationSettingsV1EvaluationSettingResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**forms** | **List[str]** |  | [optional] [readonly] 
**recommended_number_of_evaluations** | **int** |  | [optional] 
**reminder_email_schedule** | [**EvaluationApiEvaluationSettingsV1ScheduleType**](EvaluationApiEvaluationSettingsV1ScheduleType.md) |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**appraisers** | **List[str]** |  | [optional] [readonly] 
**staff_classifications** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.evaluation_api_evaluation_settings_v1_evaluation_setting_response import EvaluationApiEvaluationSettingsV1EvaluationSettingResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EvaluationApiEvaluationSettingsV1EvaluationSettingResponse from a JSON string
evaluation_api_evaluation_settings_v1_evaluation_setting_response_instance = EvaluationApiEvaluationSettingsV1EvaluationSettingResponse.from_json(json)
# print the JSON string representation of the object
print(EvaluationApiEvaluationSettingsV1EvaluationSettingResponse.to_json())

# convert the object into a dict
evaluation_api_evaluation_settings_v1_evaluation_setting_response_dict = evaluation_api_evaluation_settings_v1_evaluation_setting_response_instance.to_dict()
# create an instance of EvaluationApiEvaluationSettingsV1EvaluationSettingResponse from a dict
evaluation_api_evaluation_settings_v1_evaluation_setting_response_from_dict = EvaluationApiEvaluationSettingsV1EvaluationSettingResponse.from_dict(evaluation_api_evaluation_settings_v1_evaluation_setting_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


