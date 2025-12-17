# ValidationsApiStateReportingStepsV1UpdateStateReportingStepRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_step** | **int** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**school_year** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_state_reporting_steps_v1_update_state_reporting_step_request import ValidationsApiStateReportingStepsV1UpdateStateReportingStepRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiStateReportingStepsV1UpdateStateReportingStepRequest from a JSON string
validations_api_state_reporting_steps_v1_update_state_reporting_step_request_instance = ValidationsApiStateReportingStepsV1UpdateStateReportingStepRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiStateReportingStepsV1UpdateStateReportingStepRequest.to_json())

# convert the object into a dict
validations_api_state_reporting_steps_v1_update_state_reporting_step_request_dict = validations_api_state_reporting_steps_v1_update_state_reporting_step_request_instance.to_dict()
# create an instance of ValidationsApiStateReportingStepsV1UpdateStateReportingStepRequest from a dict
validations_api_state_reporting_steps_v1_update_state_reporting_step_request_from_dict = ValidationsApiStateReportingStepsV1UpdateStateReportingStepRequest.from_dict(validations_api_state_reporting_steps_v1_update_state_reporting_step_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


