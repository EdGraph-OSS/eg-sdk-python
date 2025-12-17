# ValidationsApiStateReportingStepsV1GetStateReportingStepsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**school_year** | **int** |  | [optional] 
**current_step** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_state_reporting_steps_v1_get_state_reporting_steps_response import ValidationsApiStateReportingStepsV1GetStateReportingStepsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiStateReportingStepsV1GetStateReportingStepsResponse from a JSON string
validations_api_state_reporting_steps_v1_get_state_reporting_steps_response_instance = ValidationsApiStateReportingStepsV1GetStateReportingStepsResponse.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiStateReportingStepsV1GetStateReportingStepsResponse.to_json())

# convert the object into a dict
validations_api_state_reporting_steps_v1_get_state_reporting_steps_response_dict = validations_api_state_reporting_steps_v1_get_state_reporting_steps_response_instance.to_dict()
# create an instance of ValidationsApiStateReportingStepsV1GetStateReportingStepsResponse from a dict
validations_api_state_reporting_steps_v1_get_state_reporting_steps_response_from_dict = ValidationsApiStateReportingStepsV1GetStateReportingStepsResponse.from_dict(validations_api_state_reporting_steps_v1_get_state_reporting_steps_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


