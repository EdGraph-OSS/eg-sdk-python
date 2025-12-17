# ValidationsApiReportingPeriodsV1SetSubmissionStatusRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**submission_id** | **str** |  | [optional] 
**status** | [**ValidationsApiReportingPeriodsV1SubmissionStatus**](ValidationsApiReportingPeriodsV1SubmissionStatus.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_set_submission_status_request import ValidationsApiReportingPeriodsV1SetSubmissionStatusRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1SetSubmissionStatusRequest from a JSON string
validations_api_reporting_periods_v1_set_submission_status_request_instance = ValidationsApiReportingPeriodsV1SetSubmissionStatusRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1SetSubmissionStatusRequest.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_set_submission_status_request_dict = validations_api_reporting_periods_v1_set_submission_status_request_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1SetSubmissionStatusRequest from a dict
validations_api_reporting_periods_v1_set_submission_status_request_from_dict = ValidationsApiReportingPeriodsV1SetSubmissionStatusRequest.from_dict(validations_api_reporting_periods_v1_set_submission_status_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


