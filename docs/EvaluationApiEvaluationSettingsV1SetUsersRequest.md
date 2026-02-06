# EvaluationApiEvaluationSettingsV1SetUsersRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**appraisers** | **List[str]** |  | [optional] [readonly] 
**staff_classifications** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.evaluation_api_evaluation_settings_v1_set_users_request import EvaluationApiEvaluationSettingsV1SetUsersRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EvaluationApiEvaluationSettingsV1SetUsersRequest from a JSON string
evaluation_api_evaluation_settings_v1_set_users_request_instance = EvaluationApiEvaluationSettingsV1SetUsersRequest.from_json(json)
# print the JSON string representation of the object
print(EvaluationApiEvaluationSettingsV1SetUsersRequest.to_json())

# convert the object into a dict
evaluation_api_evaluation_settings_v1_set_users_request_dict = evaluation_api_evaluation_settings_v1_set_users_request_instance.to_dict()
# create an instance of EvaluationApiEvaluationSettingsV1SetUsersRequest from a dict
evaluation_api_evaluation_settings_v1_set_users_request_from_dict = EvaluationApiEvaluationSettingsV1SetUsersRequest.from_dict(evaluation_api_evaluation_settings_v1_set_users_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


