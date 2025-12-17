# ValidationsApiReportingPeriodsV1ToggleSelectedRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reporting_period_id** | **str** |  | [optional] 
**selected** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_toggle_selected_request import ValidationsApiReportingPeriodsV1ToggleSelectedRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1ToggleSelectedRequest from a JSON string
validations_api_reporting_periods_v1_toggle_selected_request_instance = ValidationsApiReportingPeriodsV1ToggleSelectedRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1ToggleSelectedRequest.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_toggle_selected_request_dict = validations_api_reporting_periods_v1_toggle_selected_request_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1ToggleSelectedRequest from a dict
validations_api_reporting_periods_v1_toggle_selected_request_from_dict = ValidationsApiReportingPeriodsV1ToggleSelectedRequest.from_dict(validations_api_reporting_periods_v1_toggle_selected_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


