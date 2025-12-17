# ValidationsApiReportingPeriodsV1RunResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**category_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_run_response import ValidationsApiReportingPeriodsV1RunResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1RunResponse from a JSON string
validations_api_reporting_periods_v1_run_response_instance = ValidationsApiReportingPeriodsV1RunResponse.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1RunResponse.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_run_response_dict = validations_api_reporting_periods_v1_run_response_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1RunResponse from a dict
validations_api_reporting_periods_v1_run_response_from_dict = ValidationsApiReportingPeriodsV1RunResponse.from_dict(validations_api_reporting_periods_v1_run_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


